<template> 
   <div class="tabbar-item" @click="linkClick">
        <!-- <span class="iconfont icon-zhuye"></span>
        <div>首页</div> -->
        <!-- :style="isActives ? { color:activeColor}:{}" -->
      <div :style="isActives ? { color:activeColor}:{}">
         <slot name="content-img"></slot>
         <slot name="content"></slot> 
      </div>   
   </div>
</template>
<script>
export default {
    data() {
      return {    
         // isActive:this.isActives
      }
    },
       props:{
            link:String,
            activeColor:{
               type:String,
               default:'pink'
            }
         },
    methods: {
      linkClick(){
         this.$router.push(this.link);
      }
    },
    computed:{
        isActives(){
           return this.$route.path.includes(this.link);
         },
      
      }
}
</script>
<style scoped>
 .tabbar-item{
    flex: 1;
 }
 span {
   font-size: 25px;
 }
</style>