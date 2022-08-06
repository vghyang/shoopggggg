<template>
    <div id="tab-bar">
        <slot></slot>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
   #tab-bar {
    display: flex;
    height: 49px;
    text-align: center;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: #f3f3f3;
    align-items: center;
  }

</style>