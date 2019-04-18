<template>
  <div id="app">
    <Head2/>
    <Head1/>
    <!-- <Daohang/> -->
    <router-view/>
    <Foot1/>
  </div>
</template>
<script>
// @ is an alias to /src
import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
import Head2 from '@/components/Head2.vue'//引入路由部分(公用组件)
import Foot1 from '@/components/Foot1.vue'//引入路由部分(公用组件)
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)


export default {
  components:{
    Head1,
    Head2,
    Foot1,
    Daohang
  }
}
</script>
<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>