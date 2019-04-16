<template>
  <div class="home">
    <div class="side-bar">
      <tree-view></tree-view>
    </div>
    <div class="continer">
      <router-view />
    </div>
  </div>
</template>

<script>
import TreeView from './TreeView'
export default {
  name: 'Home',
  components:{
    TreeView
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.side-bar {
width: 300px;
height: 100%;
overflow-y: auto;
overflow-x: hidden;
font-size: 14px;
position: absolute;
top: 0;
left: 0;
}
.continer {
padding-left: 320px;
}
</style>
