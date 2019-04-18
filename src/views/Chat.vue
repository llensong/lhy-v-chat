<template>
  <div class="chat">
        <Daohang/> 
          <div class="chatAll content" >
            <div class="chatLayout float"  v-for="item in imgList">
              <div class="tit title1">{{item.name}}</div>
              <div class="img1" @click="GoToAll()">
                <img :src="item.img" alt="">
              </div>
            </div>
            
          </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Lunbotu from '@/components/Lunbotu.vue'//引入路由部分(公用组件)
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)
import Address from '@/components/Address.vue'//引入路由部分(公用组件)


import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
import Head2 from '@/components/Head2.vue'//引入路由部分(公用组件)

export default {
  name: 'home',
  components: {//引入路由部分(公用组件)
    Lunbotu,Daohang,Head1,Head2,Address
  } ,
  data(){
    return{
      imgList:[
        {name:'种植',img:require("../assets/2019/1-1.jpg")},
        {name:'养殖',img:require("../assets/2019/2-1.jpg")},
        {name:'水产',img:require("../assets/2019/4-1.jpg")},
        {name:'果木',img:require("../assets/2019/3-1.jpg")},
        {name:'花卉',img:require("../assets/2019/5-1.jpg")},
        {name:'电商',img:require("../assets/2019/6-1.jpg")}
      ]
    }
  },
  methods:{
    // 跳转到相关页面
    GoToAll(){
      this.$router.push({path:'chatAbout',query:{id:'123'}}); 
    }
  }
}
</script>
<style>
  .chat{
    width: 100%;
    height: 1000px;
    text-align: center;
  }
  .chatAll{
    margin-top: 25px;
  }
  .chatLayout{
    width: 50%;
    height: 300px;
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
    line-height: 300px;
  }
  .tit{
    width: 100%;
    height: 40px;
    line-height: 40px;
    }
  .chatLayoutContent{
    width: 100%;
    height: 260px;
  }

  .img1{
    width: 100%;
    height: 260px;
  }
  .img1 img{
    width: 80%;
    height: 100%;
  }
  .img1 img:hover{
    background:azure;
    width: 85%;
    height: 105%;
    background-color: #d7dde4
  }
</style>