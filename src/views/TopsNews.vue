<template>
    <div class="topsNews">
        <!-- <Head2/>
        <Head1/> -->
        <Daohang/>
          <div class="topsNewsContent content">
              <div class="zhengce ta-size">
                <p class="title1 top-tpls">政策</p>
                <div class="zc-list" v-for="item in zclist">
                  <div class="listimg">
                    <img :src="item.src" alt="">
                  </div>
                  <div class="listTitle">
                    <div class="a">
                      <span class="tt">{{item.title}}</span>
                    </div>
                    <div class="nexi">
                      <span class="time asp">{{item.time}}</span>                      
                      <span class="sc asp"><Icon type="md-star" /></span>
                      <span class="pl asp"><Icon type="md-text" /></span>
                      <span class="dz asp"><Icon type="md-thumbs-up" /></span></div>
                  </div>
                </div>
              </div>
              <div class="zixun ta-size">
                <p class="title1 top-tpls">资讯</p>
                <div class="zc-list" v-for="item in zxlist">
                  <div class="listimg">
                    <img :src="item.src" alt="">
                  </div>
                  <div class="listTitle">
                    <div class="a">
                      <span class="tt">{{item.title}}</span>
                    </div>
                    <div class="nexi">
                      <span class="time asp">{{item.time}}</span>                      
                      <span class="sc asp"><Icon type="md-star" /></span>
                      <span class="pl asp"><Icon type="md-text" /></span>
                      <span class="dz asp"><Icon type="md-thumbs-up" /></span></div>
                  </div>
                </div>
              </div>
              <div class="tieba ta-size">
                <p class="title1 top-tpls">提问</p>
                <div class="zc-list" v-for="item in twlist">
                  <div class="listimg">
                    <img :src="item.src" alt="">
                  </div>
                  <div class="listTitle">
                    <div class="a">
                      <span class="tt">{{item.title}}</span>
                    </div>
                    <div class="nexi">
                      <span class="time asp">{{item.time}}</span>                      
                      <span class="sc asp"><Icon type="md-star" /></span>
                      <span class="pl asp"><Icon type="md-text" /></span>
                      <span class="dz asp"><Icon type="md-thumbs-up" /></span></div>
                  </div>
                </div>
              </div>
              <div class="jishu ta-size">
                 <p class="title1 top-tpls">新技术</p>
                 <div class="zc-list" v-for="item in xjslist">
                  <div class="listimg">
                    <img :src="item.src" alt="">
                  </div>
                  <div class="listTitle">
                    <div class="a">
                      <span class="tt">{{item.title}}</span>
                    </div>
                    <div class="nexi">
                      <span class="time asp">{{item.time}}</span>                      
                      <span class="sc asp"><Icon type="md-star" /></span>
                      <span class="pl asp"><Icon type="md-text" /></span>
                      <span class="dz asp"><Icon type="md-thumbs-up" /></span></div>
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
import Address from '@/components/Address.vue'//引入路由部分(公用组件)
import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
import Head2 from '@/components/Head2.vue'//引入路由部分(公用组件)

export default {
  name: 'home',
  components: {//引入路由部分(公用组件)
    Lunbotu,Daohang,Head1,Head2,Address
  },
  data(){
    return{
      zclist:[
        {title:'发改委、农业农村部等10部委力促农村消费提质升级',time:' 14:19:15',src:require('../assets/2019/zc/1545252.jpg')},
        {title:'发改委、农业农村部等10部委力促农村消费提质升级',time:' 14:19:15',src:require('../assets/2019/zc/1545252.jpg')},
        {title:'发改委、农业农村部等10部委力促农村消费提质升级',time:' 14:19:15',src:require('../assets/2019/zc/1545252.jpg')},
        {title:'发改委、农业农村部等10部委力促农村消费提质升级',time:' 14:19:15',src:require('../assets/2019/zc/1545252.jpg')},
      ],
      zxlist:[
        {title:'未来更干净更整洁 18部门联合印发通知开展农村人居环境整治村庄清洁行动',time:' 14:19:15',src:require('../assets/2019/zc/1545356.jpg')},
        {title:'未来更干净更整洁 18部门联合印发通知开展农村人居环境整治村庄清洁行动',time:' 14:19:15',src:require('../assets/2019/zc/1545356.jpg')},
        {title:'未来更干净更整洁 18部门联合印发通知开展农村人居环境整治村庄清洁行动',time:' 14:19:15',src:require('../assets/2019/zc/1545356.jpg')},
        {title:'未来更干净更整洁 18部门联合印发通知开展农村人居环境整治村庄清洁行动',time:' 14:19:15',src:require('../assets/2019/zc/1545356.jpg')},
      ],
      twlist:[
        {title:'农村“厕所革命”怎么干，中央农办等8部门出台指导意见',time:' 14:19:15',src:require('../assets/2019/zc/1545542.jpg')},
        {title:'农村“厕所革命”怎么干，中央农办等8部门出台指导意见',time:' 14:19:15',src:require('../assets/2019/zc/1545542.jpg')},
        {title:'农村“厕所革命”怎么干，中央农办等8部门出台指导意见',time:' 14:19:15',src:require('../assets/2019/zc/1545542.jpg')},
        {title:'农村“厕所革命”怎么干，中央农办等8部门出台指导意见',time:' 14:19:15',src:require('../assets/2019/zc/1545542.jpg')},
      ],
      xjslist:[
        {title:'2019年动物疫病强制免疫计划 五种疫病划为国家强免病种',time:' 14:19:15',src:require('../assets/2019/zc/1545549.jpg')},
        {title:'2019年动物疫病强制免疫计划 五种疫病划为国家强免病种',time:' 14:19:15',src:require('../assets/2019/zc/1545549.jpg')},
        {title:'2019年动物疫病强制免疫计划 五种疫病划为国家强免病种',time:' 14:19:15',src:require('../assets/2019/zc/1545549.jpg')},
        {title:'2019年动物疫病强制免疫计划 五种疫病划为国家强免病种',time:' 14:19:15',src:require('../assets/2019/zc/1545549.jpg')},
      ]
    }
  }
}
</script>
<style>
  .topsNews{
     width: 100%;
     text-align: center;
  }
  .topsNewsContent{
    /* margin-top: 20px; */
    height: calc(100% - 50px);

    }
    .ta-size{
      width: 100%;
      height: 700px;
      margin: auto;
    }
    .zc-list{
      width: 100%;
      /* height: 100%; */
      margin: auto;
      float: left;
      height: calc((100% - 45px)/5);
      margin: 10px auto;
      font-size: 16px;
      /* margin-left: 20px; */
    }
    .zc-list .listimg{
      width: 50%;
      height: 100%;
      float: left;
    }
    .listimg img{
      width: 260px;
      height: 133px;
      margin: auto;
    }
     .listTitle{
      width: 50%;
      float: left;
    

    }
    .listTitle .a{
      width: 80%;
      height: 30px;
      word-wrap: break-word;
      /* word-break: normal; */
      text-align: justify;
      overflow:hidden; /*内容超出宽度时隐藏超出部分的内容 */
      text-overflow:ellipsis;/* 当对象内文本溢出时显示省略标记(...) ；需与overflow:hidden;一起使用。*/
      white-space:nowrap; /*不换行 */
    }
    .nexi{
       width: 80%;
       height: 30px;
       margin-top: 50px;
    }
   .asp{
     float:left;
     margin-right: 10px;
     color: darkgrey;
     }
     .top-tpls{
       /* border-bottom:1px solid; */
       /* border-color: cadetblue; */
       font-weight: 1000;
     }
</style>

