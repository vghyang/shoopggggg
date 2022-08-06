<template>
  <div id="app">
    <router-view/>
  <main-tab></main-tab>
  </div>
</template>
  <script>
  import MainTab from "components/content/mainTab/MainTab"
  export default {
    name:"App",
    components:{
      MainTab,
    }
  }
  </script>
<style>
</style>
