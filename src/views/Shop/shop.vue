<template>
    <div>
        <nav-bar class="home-nav">
            <div slot="center">购物车</div>
        </nav-bar>
    </div>
    
</template>
<script>
import NavBar from '../../components/navbar/NavBar'

export default {
    components:{
        NavBar
    }
}
</script>
<style scoped>
.home-nav{
        background-color: #FF8097;
        color:#fff
    }
</style>