<template>
    <div class="tab-bar-item" @click="itemclick">
        <slot name="item-icon"></slot>
        <div :class="{active:isActive}"><slot name="item-text"></slot></div>
    </div>
</template>
<script>
export default {
    name:"tabbaritem",
    props:{
        path:String
    },
    computed:{
        isActive(){
            return !this.$route.path.indexOf(this.path)
        }
    },
    methods:{
        itemclick(){
            this.$router.replace(this.path);
        }
    }
}
</script>
<style>
img{
    height: 24px;
    width: 24px;
    margin-top:2px;
    vertical-align: middle;
}
.tab-bar-item{
    font-size: 14px;
    flex:1;
    text-align: center;
    height: 49px;
    background-color: #f6f6f6;
}
.active{
    color:red;
}
</style>