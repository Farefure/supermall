<template>
  <div class="recommend">
    <div v-for="(item,index) in recommends" :key="index" class="recommend-item">
      <a :href="item.link">
        <img :src="item.image" />
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "RecommendView",
  props: {
    recommends: {
      type: Array,
      default() {
        return []
      }
    }
  }
}
</script>

<style>
  .recommend {
    display: flex;
    width: 100%;
    font-size: 13px;
    text-align: center;
    padding: 10px 0 23px;
    border-bottom: 10px #eee solid;
  }
  .recommend-item {
    flex: 1;
  }
  .recommend-item img {
    width: 68px;
    height: 68px;
    margin-bottom: 4px;
  }
</style>