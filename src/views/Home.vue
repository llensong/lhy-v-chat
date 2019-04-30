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
                  <p class="title1 tl">政策</p>
                  <div class="imgall float" v-for="item in imgArr">
                      <img :src="item.src" alt="">
                      <span class="inSpan">{{item.title}}</span>
                  </div>
                  <div class="allA">
                    <div class=" tlts float" v-for="item in list3">{{item}}</div>
                    <div>
                      <div class="fs float ">
                        <img src="../assets/2019/s-4.png" alt="">
                        <span class="Span">18部门联合印发通知开展农村人居环境整治村庄清洁行动</span>
                      </div>
                      <div class="float fs">
                        <table>
                          <tr class="tab" v-for="item in list4">
                            <td class="tabtd">{{item.type}} &emsp;|&emsp;</td>
                            <th class="tabth">{{item.title}}</th>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </div>
                </div>
              <div class="left1 leftContent ">
                  <p class="title1 tl">广场</p>
                  <div class="imgall float" v-for="item in imgArr">
                      <img :src="item.src" alt="">
                      <span class="inSpan">{{item.title}}</span>
                  </div>
                  <div class="allA">
                    <div class=" tlts float" v-for="item in list3">{{item}}</div>
                    <div>
                      <div class="fs float ">
                        <img src="../assets/2019/s-4.png" alt="">
                        <span class="Span">18部门联合印发通知开展农村人居环境整治村庄清洁行动</span>
                      </div>
                      <div class="float fs">
                        <table>
                          <tr class="tab" v-for="item in list4">
                            <td class="tabtd">{{item.type}} &emsp;|&emsp;</td>
                            <th class="tabth">{{item.title}}</th>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </div>
              </div>
              <div class="left1 leftContent ">
                  <p class="title1 tl">闲聊</p>
                  <div class="imgall float" v-for="item in imgArr">
                      <img :src="item.src" alt="">
                      <span class="inSpan">{{item.title}}</span>
                  </div>
                  <div class="allA">
                    <div class=" tlts float" v-for="item in list3">{{item}}</div>
                    <div>
                      <div class="fs float ">
                        <img src="../assets/2019/s-4.png" alt="">
                        <span class="Span">18部门联合印发通知开展农村人居环境整治村庄清洁行动</span>
                      </div>
                      <div class="float fs">
                        <table>
                          <tr class="tab" v-for="item in list4">
                            <td class="tabtd">{{item.type}} &emsp;|&emsp;</td>
                            <th class="tabth">{{item.title}}</th>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </div>
              </div>
              <div class="left1 leftContent ">
                  <p class="title1 tl">新技术</p>
                  <div class="imgall float" v-for="item in imgArr">
                      <img :src="item.src" alt="">
                      <span class="inSpan">{{item.title}}</span>
                  </div>
                  <div class="allA">
                    <div class=" tlts float" v-for="item in list3">{{item}}</div>
                    <div>
                      <div class="fs float ">
                        <img src="../assets/2019/s-4.png" alt="">
                        <span class="Span">18部门联合印发通知开展农村人居环境整治村庄清洁行动</span>
                      </div>
                      <div class="float fs">
                        <table>
                          <tr class="tab" v-for="item in list4">
                            <td class="tabtd">{{item.type}} &emsp;|&emsp;</td>
                            <th class="tabth">{{item.title}}</th>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </div>
              </div>
            </div>
            <div class="rights1 float">
              <div class="right1 rightContent">
                <p class="title1 tl">周榜热点</p>
                <ul class="titleContnet">
                  <li class="titleContnet-item " v-for="item in list2">
                    <a href="">
                      <i class="focus_num">1</i>
                      <span>{{item}}</span>
                    </a>
                  </li>
                </ul>
              </div>
              <div class="right1 rightContent reci">
              <div class="title1 tl">今日热词</div>
              <div class="item " v-for="item in list5">
                <a href="" class="a-word">
                  {{item}}
                </a>
              </div>
              </div>
              <div class="right1 rightContent">
                <p class="title1 tl">好文推荐</p>
                <ul class="titleContnet">
                  <li class="titleContnet-item " v-for="item in list2">
                    <a href="">
                      <i class="focus_num">1</i>
                      <span>{{item}}</span>
                    </a>
                  </li>
                </ul>
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
      list:['种植','养殖','水产','果木','花卉','电商'],
      list2:[
        "远程医疗平台计划覆盖2277个贫困村",
        "社区+旅游：第三代露营地的发展趋势",
        "2019年四大粮食作物的价格走势，玉米最值得看好！",
        "2019年起这些新规将影响你的生活",
        "12月我国部分农产品供需形势分析"
      ],
      imgArr:[
        {
          title:"抓紧抓实“三农”大事要事急事难事",
          src:require('../assets/2019/s-1.jpg'),
         },
         {
          title:"为什么要坚持农业农村优先发展？",
          src:require('../assets/2019/s-2.jpg'),
         },
         {
          title:"农田休耕轮作提升京郊农户种植效益",
          src:require('../assets/2019/s-3.jpg'),
         },
        //  {
        //   title:"18部门联合印发通知开展农村人居环境整治村庄清洁行动",
        //   src:require('../assets/2019/s-4.png'),
        //  }
      ],
      list3:[
        "种植新说","养殖有道","问题求解","掌握新技术"
      ],
      list4:[
         { type:"热点",title:"力争2020年化肥农药使用量实现负增长"},
         { type:"最新",title:"关于公布2018年稻谷最低收购价格的通知"},
         { type:"提问",title:"关于公布2018年小麦最低收购价格的通知"},
         { type:"政策",title:"全国休闲农业和乡村旅游大会在江苏召开"},
         { type:"新闻",title:"违规“大棚房”装不下“田园梦”！"}
      ],
      list5:[
          "农村电商","土地承包","畜牧业扶持政策","夏粮收购",
          "农业补贴","农业一号文件","猪肉价格","粮食供求",
          "农业土地政策","扶贫资金","临储小麦玉米","临储农业政策","农业保险水肥一体化"
      ]
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
        min-width: 721px;
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
    .cons .rights1 .right1{
      width: 80%;
      margin: auto;
    }
    .imgall{
      text-align:center;
      margin-top:25px;
      width: 240px;
      height: 139px;
      position: relative;
      float: left;
      margin-left: 45px;
    }
    .imgall img{
      width: 210px;
      height: 139px;
    }
    .inSpan{
      position: absolute;
      left: 14px;
      bottom: 0;
      width: 212px;
      padding: 0 10px;
      height: 29px;
      line-height: 29px;
      color: #fff;
      background-color: rgba(0,0,0,0.5);
      overflow:hidden; /*内容超出宽度时隐藏超出部分的内容 */
      text-overflow:ellipsis;/* 当对象内文本溢出时显示省略标记(...) ；需与overflow:hidden;一起使用。*/
      white-space:nowrap; /*不换行 */
    }
    .tl{
      text-align: center;
      text-justify: newspaper;
      border-bottom: 7px solid
    }
    .tr{
      border-bottom: 3px solid;
    }
    .titleContnet{
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
    }
    .titleContnet a:link span {
      font-size: 16px;
      color: #444;
      padding-left: 5px;
    } 
    .titleContnet-item {
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
      word-wrap: break-word; 
      word-break: normal;
      text-align: justify;
      text-justify: newspaper;
      }

    .titleContnet-item a:link .focus_num {
        display: inline-block;
        font-size: 12px;
        width: 16px;
        height: 16px;
        text-align: center;
        line-height: 16px;
        background: #A8DDC7;
        border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px;
        font-style: normal;
        color: #fff;
        margin-right: 2px;
        float: left;
        margin-top: 4px;
    }
    .allA{
         width: 100%;
        margin-top: 177px;
        margin: auto;
      
    }
    .tlts{
      width: 25%;
      border-bottom: 4px solid;
      border-color: rgb(28, 219, 38);
      border-width: 50%;
      color: rgba(7, 173, 71, 0.897);

    }
    .tlts:hover{
      border-bottom: 4px solid;
      border-color: rgb(3, 128, 41);
      color: rgb(133, 197, 171);
    }
    .fs{
      margin-top: 19px;
      margin-left: 60px;
      position: relative;
    }
    .tabtd{
      color: rgb(3, 202, 119);
       height: 30px;
      font-size: 15px;
    }
    .tabth{
      text-align: justify;
      color: #212122;
      height: 30px;
      font-size: 15px;
      font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif
    }
    .Span{
      position: absolute;
      left: 0px;
      bottom: 7px;
      width: 212px;
      padding: 0 10px;
      height: 39px;
      line-height: 17px;
      color: #fff;
      background-color: rgba(0,0,0,0.5);
      overflow:hidden; /*内容超出宽度时隐藏超出部分的内容 */
      text-overflow:ellipsis;/* 当对象内文本溢出时显示省略标记(...) ；需与overflow:hidden;一起使用。*/
      white-space:nowrap; /*不换行 */
    }
    .item{
      margin-top: 20px;
    }
    .a-word{
      padding: 0px 9px;
      height: 22px;
      line-height: 22px;
      background: #dcf2e5;
      font-size: 14px;
      color: #46A87F;
      display: block;
      float: left;
      margin-right: 6px;
      margin-bottom: 8px;
      border-radius: 2px;
      -moz-border-radius: 2px;
    }
    .reci{
      height: 250px;
    }
    .lefts1 {
    width: 68%;
    height: 100%;
    margin: auto;
    /* border-right: 1px solid; */
    /* border-right-color: rgba(174, 235, 240, 0.884); */
    margin-top: 50px;
    /* height: 1200px; */
}

.rights1 {
    height: 100%;
    width: 32%;
    margin: auto;
    margin-top: 50px
}

.leftContent {
    width: 100%;
    height: 442px;
    /* height: 33%; */
    margin-bottom: 30px;
}

.rightContent {
    width: 100%;
    /* height: 33%; */
}
.ivu-carousel-item{
    width: 100%; 
    height: auto;
    left: 0px;
}
</style>
