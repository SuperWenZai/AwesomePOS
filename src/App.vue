<template>
  <div id="app">
    <left-nav></left-nav>
    <div class="main">
      <keep-alive>
         <router-view></router-view>
      </keep-alive>
    </div>

  </div>
</template>

<script>
import leftNav from '@/components/common/leftNav'
export default {
  name: 'app',
  data(){
    return{}
  },
  components : {
    leftNav
  }
}
</script>

<style lang="less" scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  .main {
    height: 100%;
    width: 95%;
    float: right;
    background-color: #EFF2F7;
    overflow: hidden;
  }
}
</style>

