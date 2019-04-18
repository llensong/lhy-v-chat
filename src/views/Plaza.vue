<template>

    <div class="plaza">
        <!-- <Head2/>
        <Head1/> -->
        <Daohang/>
        <div class="allPlaza">   
            <div class="one">
                <div>
                    <div class="title1">问答</div>
                </div>
            </div>
            <div class="one title1">热帖</div>
            <div class="one title1">聚焦</div>
            <div class="one title1">关注</div>
           
        </div>
    </div>
</template>
<script>
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)
import Address from '@/components/Address.vue'//引入路由部分(公用组件)

export default {
    components: {//引入路由部分(公用组件)
        Address,Daohang
    }
}
</script>
<style>
    .plaza{
        height: 100%;
        text-align: center;
    }
    .allPlaza{
        width: 80%;
        margin: auto;
        background-color: rgba(149, 229, 225, 0.486);
    }
    .one{
        width:  100%;
        height: 400px;
        border-bottom: solid 2px;
        border-bottom-color: azure;
        border-bottom-left-radius: 5px ;
        border-bottom-right-radius: 5px ;
    }
   
</style>
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
  }
}
</script>
