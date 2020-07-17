<template>
  <div>首页</div>
</template>
<script>
import axios from "axios";

export default {
  name: "Home",
  data() {
    return {
      result: ""
    };
  },
  created() {
    axios({
      url: "http://123.207.32.32:8000/home/multidata",
      method: "get"
    }).then(res => {
      this.result = res;
      console.log(result);
    });
  }
};
</script>
<style scoped>
</style>
