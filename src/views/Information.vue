<template>
    <div class="information">
        <!-- <Head2/>
        <Head1/> -->
        <Daohang /> 
        <div class="mation">
         <Layout>
            <Header>
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <!-- <div class="layout-logo">资讯</div> -->
                    <div class="layout-nav">
                        <!-- <MenuItem name="1">
                            <Icon type="ios-navigate"></Icon>
                            新闻
                        </MenuItem> -->
                        <MenuItem name="2">
                            <Icon type="ios-keypad"></Icon>
                            头条
                        </MenuItem>
                        <MenuItem name="3">
                            <Icon type="ios-analytics"></Icon>
                           热点
                        </MenuItem>
                        <MenuItem name="4">
                            <Icon type="ios-leaf" />
                            种植
                        </MenuItem>
                        <MenuItem name="4">
                            <Icon type="logo-steam" />
                            养殖
                        </MenuItem>
                         <MenuItem name="4">
                            <Icon type="ios-podium" />
                            全部
                        </MenuItem>
                    </div>
                </Menu>
            </Header>
            <Content :style="{padding: '0 50px'}">
              
                <Card>
                    <div class="MationContent">
                        <div class="ToNew">
                           <div class="lbt3 today">
                                <Carousel autoplay v-model="value3" loop>
                                    <CarouselItem v-for="item in listArr">
                                        <div class="demo-carousel"><img style="width:600px;height:330px" :src="item" alt=""></div>
                                    </CarouselItem>
                                </Carousel>
                            </div>
                            <div class="day2 today">
                                <div class="todayTitle title1">
                                    今日关注
                                </div>
                                <hr>
                                <div class='todayContent'>
                                    <ol >
                                        <li></li>
                                        <li></li>
                                        <li></li>
                                        <li></li>
                                    </ol>
                                </div>
                            </div>
                        </div>
                         <div class="new">
                            
                        </div>
                         <div class="new">
                            
                        </div>
                         <div class="new">
                            
                        </div>
                         <div class="new">
                            
                        </div>

                    </div>
                </Card>
            </Content>
        </Layout>
        </div>
    </div>
</template>
<script>
// @ is an alias to /src
// import Lunbotu from '@/components/Lunbotu.vue'//引入路由部分(公用组件)
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)
import Address from '@/components/Address.vue'//引入路由部分(公用组件)
import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
import Head2 from '@/components/Head2.vue'//引入路由部分(公用组件)


export default {
  name: 'home',
  components: {//引入路由部分(公用组件)
    // Lunbotu,
    Daohang,
    Head1,
    Head2,
    Address
  },  
 data () {
            return {
                value3: 0,
                listArr:[
                require("../assets/2019/779.jpg"),
                require("../assets/2019/780.jpg"),
                require("../assets/2019/782.jpg"),
                // require("../assets/2019/779.jpg"),
                // require("../assets/2019/779.jpg")
               ]
            }
        },
}
</script>
<style>
    .information{
        width: 100%;
        text-align: center;
    }
    .ivu-menu-horizontal .ivu-menu-item, .ivu-menu-horizontal .ivu-menu-submenu {
    float: left;
    padding: 0px 5px;
    position: relative;
    cursor: pointer;
    z-index: 3;
    transition: all .2s ease-in-out;
    }
    .ivu-card-body {
    padding: 0;
    }
    .mation{
        width: 90%;
        margin: auto;
        background-color: antiquewhite
    }
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
    }
    .layout-nav{
        width: 420px;
        margin: 0 auto;
        margin-right: 20px;
    }
    .layout-footer-center{
        text-align: center;
    }
    /* .lbt2 {
       width: 400px;
       height: 300px;
   } */
   .lbt2 ivu-carousel{
       width: 100%;
       height: 100%;
          }
    .ToNew{
        width: 99%;
        height: 350px;
        margin: auto;
        text-align: center;
    }
     .day2{
        width: 38%;
        height: 90%;
        margin-left: 19px;
        margin-top: 35px;
    }
    .lbt3{
         width:52%;
        height:100%;
        margin-top: 30px;
    }
    .new{
         width: 100%;
        height: 300px;
    }
    
    ol{
        list-style-type: square;
    }
    
</style>
