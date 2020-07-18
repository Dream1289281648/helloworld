<template>
  <div>
    <nav-bar class="home-nav">
      <div slot="center">首页</div>
    </nav-bar>
  </div>
</template>
<script>
import axios from "axios";
import NavBar from "../../components/navbar/NavBar";

export default {
  name: "Home",
  data() {
    return {
      result: ""
    };
  },
  components: {
    NavBar
  },
  created() {
    axios({
      url: "http://123.207.32.32:8000/home/multidata",
      method: "get"
    }).then(res => {
      this.result = res;
      console.log(this.result.data);
    });
  }
};
</script>
<style scoped>
.home-nav {
  background-color: #ff8097;
  color: #fff;
}
</style>
