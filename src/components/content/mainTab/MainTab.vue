<template>
      <tab-bar>
    <tab-bar-item link='/home'>
      <template v-slot:content-img >
        <span class="iconfont icon-zhuye"></span>
      </template>
      <template v-slot:content>
        <div>首页</div>
      </template>
    </tab-bar-item>

    <tab-bar-item link="/category">
      <template v-slot:content-img>
        <span class="iconfont icon-fenlei"></span>
      </template>
      <template v-slot:content>
        <div>分类</div>
      </template>
    </tab-bar-item>
    
    <tab-bar-item link="/cart">
      <template v-slot:content-img>
        <span class="iconfont icon-gouwuche"></span>
      </template>
      <template v-slot:content>
        <div>购物车</div>
      </template>
    </tab-bar-item>

     <tab-bar-item link="/profile">
      <template v-slot:content-img>
        <span class="iconfont icon-wode"></span>
      </template>
      <template v-slot:content>
        <div>我的</div>
      </template>
    </tab-bar-item>
   </tab-bar>
</template>

<script>
import TabBar from "components/common/tabbar/TabBar";
import TabBarItem from 'components/common/tabbar/TabBarItem'
export default {
    components:{
        TabBar,
        TabBarItem
        
    }
}
</script>

<style scoped>

</style>