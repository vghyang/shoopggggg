<template>
  <div class="recommend">
    <div v-for="(item,index) in recommends" class="recommend-item" :key="index">
      <a :href="item.link">
        <img :src="item.image" alt="">
        <div class="title">{{item.title}}</div>
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

<style scoped>
 .recommend{
  display: flex;
  padding: 10px 0 20px;
  border-bottom: 10px solid #eee;
 }

 .recommend-item {
  flex: 1;
  text-align: center;
 }
  .recommend-item  .title {
    margin-top: 8px;
  }
 .recommend img {
    width: 100%;
 }
</style>
