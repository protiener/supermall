<template>
  <div class="nav-bar">
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
  export default {
    name: "NavBar"
  }
</script>

<style scoped>
  .nav-bar{
    height: 44px;
    display: flex;
    line-height: 44px;
    text-align: center;
  }
  .left {
    width: 60px;
  }
  .center {
    flex: 1;
  }
  .right {
    width: 60px;
  }
</style>
