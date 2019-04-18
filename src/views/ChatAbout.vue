<template>
  <div class="chatAbout">
        <Daohang/> 
        <div class="content">
          <div class="headAll">
              <div class="headTitle">
                <img src="" alt="">
                  <div>
                    <div>名称</div>
                    <div>管理员</div>
                    <div>帖子数量</div>
                    <div>目录</div>
                  </div>
            </div>
            <div class="headContent">
              <div>
                <Input search enter-button placeholder="吧内搜索" />
              </div>
              <div>
                <div class="title1">疑难解答</div>
                <div class="ProblemContent">
                  <ol>
                    <li></li>
                  </ol>
                </div>
              </div>
              <div>
                <div class="title1">热门话题</div>
                <div class="topContent">
                  <ol>
                    <li></li>
                  </ol>
                </div>
              </div>
            </div>
          </div>
          <div class="ChatAboutContent">
            <div class="AboutContent">
              <div class="paixu">
                <Cascader :data="data" change-on-select></Cascader>
              
              </div>
              <div class="AboutContentHead">
                <div>评论总数</div>
                <div>帖子类型</div>
                <div>帖子名称</div>
                <div>发帖人</div>
              </div>
              <div class="A-Content">
                <div>简单介绍</div>
                <div>发帖时间</div>
              </div>
            </div>
          </div>
          <div class="toPic">
            <div class="toPicTitle">
              <Input v-model="value1" size="small" placeholder="请输入话题" />
              </div>
            <div class="toPicContent">
              <Input v-model="value1" size="large" placeholder="请输入话题内容" />
            </div>
            <button type="submit">发表</button>
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
       data: [
         {
              value: '热度',
              label: '热度',
              children: [
                  {
                      value: '升序',
                      label: '升序'
                  },
                  {
                      value: '降序',
                      label: '降序'
                  }
              ]
          },
          {
              value: '时间',
              label: '时间',
              children: [
                  {
                      value: '升序',
                      label: '升序'
                  },
                  {
                      value: '降序',
                      label: '降序'
                  }
              ]
          },
          ], 
       }
  },
  methods:{
    // 跳转到相关页面
    GoToAll(){
      this.$router.push({path:'',query:{id:'123'}}); 
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