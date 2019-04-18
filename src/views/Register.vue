<template>
  <div class="regist">
    <!-- <Head2/>
    <Head1/> -->
    <div class="registContent">
      <form action>
          <table>
            <tr>
              <th>用户名:</th>
              <td>
                <input type="text" name="" id="">
              </td>
            </tr>
             <tr>
              <th>密码:</th>
              <td>
                <input type="password" name="" id="">
              </td>
            </tr>
             <tr>
              <th>确认密码:</th>
              <td>
                <input type="password" name="" id="">
              </td>
            </tr>
             <tr>
              <th>验证码:</th>
              <td>
                <img src="" alt="">换一张
              </td>
            </tr>
             <tr>
              <th>请输入验证码:</th>
              <td>
                <input type="text" name="" id="">
              </td>
            </tr>
          </table>
      </form>
    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import Lunbotu from "@/components/Lunbotu.vue"; //引入路由部分(公用组件)
import Daohang from "@/components/Daohang.vue"; //引入路由部分(公用组件)

import Head1 from "@/components/Head1.vue"; //引入路由部分(公用组件)
import Head2 from "@/components/Head2.vue"; //引入路由部分(公用组件)

export default {
  name: "home",
  components: {
    //引入路由部分(公用组件)
    Lunbotu,
    Daohang,
    Head1,
    Head2
  }
};
</script>
<style>
  .regist{
    width:100%;
    height: 600px;

  }
  .registContent{
    background-color: cadetblue;
    width: 70%;
    height: 100%;
    margin: auto;
  }
  form{
    width: 80%;
    height: 100%;
    margin: auto;
  }
  table{
    width: 100%;
    height: 100%;
  }
</style>
