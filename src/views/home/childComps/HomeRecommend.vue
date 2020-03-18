<template>
  <div class="recommend">
    <div class="recommend-item" v-for="item in recommends">
      <a :href="item.link">
        <img :src="item.image" alt="">
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "HomeRecommend",
    props: {
      recommends: {
        type: Array,
        default() {
          return [];
        }
      }
    }
  }
</script>

<style scoped>
  .recommend {
    width: 100%;
    display: flex;
    align-items: center;
    justify-items: center;
    text-align: center;
  }

  .recommend-item {
    flex: 1;
    margin: 8px 0;
  }
  .recommend-item img {
    width: 70px;
    height: 70px;
    margin-bottom: 5px;
  }
  .recommend-item div {
    font-size: var(--font-size);
  }
</style>
