<template>

    <div class="plazza">
        <!-- <Head2/>
        <Head1/> -->
        <Daohang/>
        <div class="allplazza">   
            <div class="one">
                <div class="plaz-heade ">
                    <div class="plaz-hel">
                        <img class="float hls" src="../assets/2019/huo.jpg" alt=""> 
                        <p class="title1 float hls">问答</p> 
                    </div>
                    
                </div>
                <div class="plaz-list">
                    <ul class="plaz-Contnet">
                        <li class="plaz-Contnet-item " v-for="item in list">
                            <div class="a">
                                <i class="focus_num">{{item.type}}</i>
                                <span class="aspan">{{item.title}}</span>
                                <!-- <span class="sc plaz-asp"><Icon type="md-star" /></span> -->
                                <span class=" plaz-asp">{{item.num}}</span>
                                <span class="pl plaz-asp"><Icon type="md-text" /></span>
                                <!-- <span class="dz plaz-asp"><Icon type="md-thumbs-up" /></span> -->
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="one">
                <div class="plaz-heade ">
                    <div class="plaz-hel">
                        <img class="float hls" src="../assets/2019/huo.jpg" alt=""> 
                        <p class="title1 float hls">热帖</p> 
                    </div>
                    
                </div>
                <div class="plaz-list">
                    <ul class="plaz-Contnet">
                        <li class="plaz-Contnet-item " v-for="item in list">
                            <div class="a">
                                <i class="focus_num">{{item.type}}</i>
                                <span class="aspan">{{item.title}}</span>
                                <!-- <span class="sc plaz-asp"><Icon type="md-star" /></span> -->
                                 <span class=" plaz-asp">{{item.num}}</span>
                                <span class="pl plaz-asp"><Icon type="md-text" /></span>
                                <!-- <span class="dz plaz-asp"><Icon type="md-thumbs-up" /></span> -->
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="one">
                <div class="plaz-heade ">
                    <div class="plaz-hel">
                        <img class="float hls" src="../assets/2019/huo.jpg" alt=""> 
                        <p class="title1 float hls">聚焦</p> 
                    </div>
                    
                </div>
                <div class="plaz-list">
                    <ul class="plaz-Contnet">
                        <li class="plaz-Contnet-item " v-for="item in list">
                            <div class="a">
                                <i class="focus_num">{{item.type}}</i>
                                <span class="aspan">{{item.title}}</span>
                                <!-- <span class="sc plaz-asp"><Icon type="md-star" /></span> -->
                                 <span class=" plaz-asp">{{item.num}}</span>
                                <span class="pl plaz-asp"><Icon type="md-text" /></span>
                                <!-- <span class="dz plaz-asp"><Icon type="md-thumbs-up" /></span> -->
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="one">
                <div class="plaz-heade ">
                    <div class="plaz-hel">
                        <img class="float hls" src="../assets/2019/huo.jpg" alt=""> 
                        <p class="title1 float hls">关注</p> 
                    </div>
                    
                </div>
                <div class="plaz-list">
                    <ul class="plaz-Contnet">
                        <li class="plaz-Contnet-item " v-for="item in list">
                            <div class="a">
                                <i class="focus_num">{{item.type}}</i>
                                <span class="aspan">{{item.title}}</span>
                                <span class="sc plaz-asp"><Icon type="md-star" /></span>
                                 <span class=" plaz-asp">{{item.num}}</span>
                                <span class="pl plaz-asp"><Icon type="md-text" /></span>
                                 <span class=" plaz-asp">{{item.num}}</span>

                                <span class="dz plaz-asp"><Icon type="md-thumbs-up" /></span>

                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="one">
                <div class="plaz-heade ">
                    <div class="plaz-hel">
                        <img class="float hls" src="../assets/2019/huo.jpg" alt=""> 
                        <p class="title1 float hls">城市</p> 
                    </div>
                    
                </div>
                <div class="plaz-list">
                    <ul class="plaz-Contnet">
                        <li class="plaz-Contnet-item " v-for="item in list">
                            <div class="a">
                                <i class="focus_num">{{item.type}}</i>
                                <span class="aspan">{{item.title}}</span>
                                <!-- <span class="sc plaz-asp"><Icon type="md-star" /></span> -->
                                <span class=" plaz-asp">{{item.num}}</span>
                                <span class="pl plaz-asp"><Icon type="md-text" /></span>
                                <!-- <span class="dz plaz-asp"><Icon type="md-thumbs-up" /></span> -->
                            </div>
                        </li>
                    </ul>
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
  data(){
      return{ 
            list:[
                {type:"农业技术 种植",title:"栽种得小麦根部有白毛是什么问题？",num:20},
                {type:"生活 其他",title:"是黑暗要将至了吗？刚写了一个帖子，被秒删是黑暗要将至了吗？刚写了一个帖子，被秒删",num:20},
                {type:"农业技术 种植",title:"栽种得小麦根部有白毛是什么问题？",num:20},
                {type:"农业技术 种植",title:"栽种得小麦根部有白毛是什么问题？",num:20},
                {type:"农业技术 种植",title:"栽种得小麦根部有白毛是什么问题？",num:20},

            ],
        }
  }
}
</script>
<style>
    .plazza{
        height: 100%;
        text-align: center;
    }
    .allplazza{
        width: 70%;
        margin: auto;
        /* background-color: rgba(198, 253, 223, 0.486); */

    }
    .one{
        width:  100%;
        height: 400px;
        margin: 30px auto;
        border-bottom: solid 2px;
        border-bottom-left-radius: 15px ;
        border-bottom-right-radius: 15px ;
        border-top: solid 2px;
        border-top-left-radius: 15px ;
        border-top-right-radius: 15px ;
        border-color: aliceblue;
        background-color: rgba(149, 229, 225, 0.486);

    }
    .plaz-heade{
        width: 100%;
        height: 30px;
        text-align: center;
        margin: auto;
        margin-top: 20px;
    }
   
   .plaz-hel{
       width: 20%;
       height: 100%;
       margin: auto; 
    }
   .plaz-hel img{
    width: 30px;
    height: 30px;
   }
   .hls{
       margin-left: 30px;
   }
   .plaz-list{
       width: 90%;
       margin: auto;
       text-align: center;
   }
     .pl-content{
        width: 70%;
        margin: auto;
        background-color: azure;
    }
     .plaz-Contnet{
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
    }
    .plaz-Contnet .a  .aspan {
      font-size: 16px;
      color: #444;
      padding-left: 5px;
      width: 400px;
      overflow: hidden;
      text-overflow: ellipsis;
      word-wrap: normal;
    } 
    .plaz-Contnet-item {
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
      word-wrap: break-word; 
      word-break: normal;
      text-align: justify;
      text-justify: newspaper;
      overflow:hidden; /*内容超出宽度时隐藏超出部分的内容 */
      text-overflow:ellipsis;/* 当对象内文本溢出时显示省略标记(...) ；需与overflow:hidden;一起使用。*/
      white-space:nowrap; /*不换行 */
      }

    .plaz-Contnet-item .a .focus_num {
        displazy: inline-block;
        /* font-size: 12px; */
        width: 100px;
        /* height: 16px; */
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
    .plaz-asp{
     float:right;
     margin-right: 10px;
     color: darkgrey;
     }
</style>
