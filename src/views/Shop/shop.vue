<template>
  <div>
    <nav-bar class="home-nav">
      <div slot="center">购物车</div>
    </nav-bar>
  </div>
</template>
<script>
import NavBar from "../../components/navbar/NavBar";

// // 引入全部组件
// import Vue from "vue";
// import Mint from "mint-ui";
// Vue.use(Mint);
// // 按需引入部分组件
// import { Cell, Checklist } from "mint-ui";
// Vue.component(Cell.name, Cell);
// Vue.component(Checklist.name, Checklist);

// import { Actionsheet } from "mint-ui";
// Vue.component(Actionsheet.name, Actionsheet);

export default {
  data() {
    return {};
  },
  components: {
    NavBar
  }
};
</script>
<style scoped>
.home-nav {
  background-color: #ff8097;
  color: #fff;
}
</style>