<template>
    <div class="topsNews">
        <!-- <Head2/>
        <Head1/> -->
        <Daohang/>
          <div class="topsNewsContent content">
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
  }
}
</script>
<style>
  .topsNews{
     width: 100%;
     height: 1200px;
     text-align: center;
  }
  .topsNewsContent{
    /* margin-top: 20px; */
    height: calc(100% - 50px);

    }
 
</style>

