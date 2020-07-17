<template>
  <div id="app">
    <tab-bar>
      <tab-bar-item path="/home">
        <img slot="item-icon" src="@/assets/1.png" />
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img slot="item-icon" src="@/assets/1.png" />
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/shop">
        <img slot="item-icon" src="@/assets/1.png" />
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img slot="item-icon" src="@/assets/1.png" />
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
    <router-view></router-view>
  </div>
</template>
<script>
import TabBar from "./components/tabbar/tabbar";
import TabBarItem from "./components/tabbar/tabbaritem";

export default {
  components: {
    TabBar,
    TabBarItem
  }
};
</script>
<style>
* {
  margin: 0;
  padding: 0;
}
</style>
