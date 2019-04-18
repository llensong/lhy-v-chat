<template>
  <div class="home">
    <!-- //引入路由部分(公用组件) -->
    <Daohang /> 
    <div class="layout ">
        <!-- <div class="layout-ceiling">
            <div class="layout-ceiling-main">
                <router-link to="/">服务大厅</router-link>|
                <a href="#">个人中心</a>
            </div>
        </div> -->
        <div class="layout-header" >
            <div class="layout-logo">
              <img src="" alt="">
            </div>
            <div class="layout-logo" v-for="item in list" @click="GoToAbout()">{{item}}</div>
        </div>
        <div  class="cons">
            <Lunbotu/>
              <div class="lefts1 float">
                <div class="left1 leftContent ">
                  <div class="title1">
                  12345667878
                  </div>
                  <div class="title1">
                    12345667878
                  </div>
                </div>
                <div class="left2 leftContent ">
                  <div class="title1">
                  12345667878
                  </div>
                  <div class="title1">
                    12345667878
                  </div>
                </div>
                <div class="left3 leftContent ">
                  <div class="title1">
                  12345667878
                  </div>
                  <div class="title1">
                    12345667878
                  </div>
                </div>
                <div class="left4 leftContent ">
                  <div class="title1">
                  12345667878
                  </div>
                  <div class="title1">
                    12345667878
                  </div>
                </div>
            </div>
            <div class="rights1 float">
              <div class="right1 rightContent">
                <div class="title1">
                周榜热点
                </div>
                <div class="weekNews">
                  <ol>
                    <li></li>
                    <li></li>
                    <li></li>
                  </ol>
                </div>
              </div>
              <div class="right1 rightContent">
                <div class="title1">
                12345667878
                </div>
                <div class="title1">
                  12345667878
                </div>
              </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Lunbotu from '@/components/Lunbotu.vue'//引入路由部分(公用组件)
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)

import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
import Head2 from '@/components/Head2.vue'//引入路由部分(公用组件)

export default {
  name: 'home',
  components: {//引入路由部分(公用组件)
    Lunbotu,Daohang,Head1,Head2
  },
  data() {
    return {
      list:['种植','养殖','水产','果木','花卉','电商']
    }
  },
  methods:{
    GoToAbout(){
      this.$router.push({path:'seach',query:{id:'123'}}); 
    }
  }
}
</script>
<style>
 .layout{
        border: 1px solid #d7dde4;
        background: #f5f7f9;
        position: relative;
        border-radius: 4px;
        overflow: hidden;
    }
    .layout-logo{
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
        color: #f5f7f9;
        line-height: 30px;
        cursor: pointer;
    }
    .layout-header{
        height: 60px;
        background: #fff;
        box-shadow: 0 1px 1px rgba(0,0,0,.1);
    }
    
    .layout-ceiling {
      background: cadetblue;;
      /* padding: 10px 0; */
      overflow: hidden;
      height: 50px;
      line-height: 50px;
    }
    .layout-ceiling-main{
        float: right;
        margin-right: 15px;
    }
    .layout-ceiling-main a{
        color: #9ba7b5;
    }
    .cons{
      width: 85%;
      margin: auto;
    }
</style>
