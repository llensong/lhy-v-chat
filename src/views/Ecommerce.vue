<template>
    <div class="ecommerce">
        <Daohang/>
        <!-- <div class="ecommerceAll"> -->
            <div class=" content">
              <div class="ecall" v-for="item in list">
                <div class="ectitle title1">{{item}}</div>
                <hr>
                <div class="ecContent content">内容</div>
              </div>
            </div>
        <!-- </div> -->
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
      list:[
        '农产品','农业工具','培育技术'
      ]
    }
  }
}
</script>
<style>
  .ectitle{

  }
</style>
