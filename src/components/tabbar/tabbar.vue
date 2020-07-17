<template>
  <div id="tab-bar">
      <slot></slot>
  </div>
</template>
<script>
export default {
    name:"tabbar"
}
</script>
<style scoped>
#tab-bar{
    display:flex;
    position: absolute;
    right: 0;
    left: 0;
    bottom: 0;
}
</style>
