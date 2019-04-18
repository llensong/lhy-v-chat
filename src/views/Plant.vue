<template>
    
    <div class="plant">
       <!-- <Head2/>
        <Head1/>  -->
        <Daohang/>
        <div class="content">
            <div class="ToNew">
                <div class="lbt2 float">
                    <Carousel autoplay v-model="value3" loop>
                        <CarouselItem v-for="item in listArr">
                            <div class="demo-carousel">
                                <img style="width:600px;height:350px" :src="item" alt="">
                            </div>
                        </CarouselItem>
                    </Carousel>
                </div>
                <div class="day float">
                    <div class="todayTitle title1">
                        新政策
                    </div>
                    <hr>
                    <div class='todayContent'>
                        <ol >
                            <li @click="gotoDetails()">1</li>
                            <li>2</li>
                            <li>3</li>
                            <li>4</li>
                        </ol>
                    </div>
                </div>
            </div>
            <div class="new">
                1
            </div>
            <div class="new">
                2
            </div>
            <div class="new">
                3 
            </div>
            <div class="new">
                4 
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
  data () {
            return {
                value3: 0,
                listArr:[
                require("../assets/2019/343-1.jpg"),
                require("../assets/2019/367-1.jpg"),
                require("../assets/2019/568-1.jpg"),
                // require("../assets/2019/779.jpg"),
                // require("../assets/2019/779.jpg")
               ]
            }
        },
    methods:{
        gotoDetails(){
            this.$router.push({path:'Details',query:{id:'1'}})
        }
    }
}
</script>
<style>
    .plant{
    width: 100%;
    /* background-color: azure */
    }
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
    .day{
        width: 41%;
        height: 90%;
        margin-left: 19px;
        margin-top: 35px;
    }
    .lbt2{
         width:54%;
        height:100%;
        margin-top: 30px;
    }
   
    .new{
         width: 100%;
        height: 300px;
    }
    .ivu-carousel-list {
        position: relative;
        display: block;
        overflow: hidden;
        margin: 0;
        padding: 0;
        width: 100%;
        height: 100%;
    }
    .ivu-carousel {
        position: relative;
        display: block;
        box-sizing: border-box;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
        touch-action: pan-y;
        -webkit-tap-highlight-color: transparent;
        width: 100%;
        height: 90%;
    }
</style>
