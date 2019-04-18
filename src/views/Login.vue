<template>
    <div class="login">
        <!-- <Head2/>
        <Head1/> -->

         <br>
        <div class="iform">
                    <h3>着手看天下，交流改变生活</h3>
            <div class="loginabout">
                <img src="../assets/1.jpg" alt="">
            </div>
            <div class="loginform">
                <div class="loginOne">
                    <div class="form">
                        <div class="loginTitle"> 
                            用户名&#8194;|&#8194;
                        </div>
                        <i-input :value.sync="value" placeholder="请输入用户名" ></i-input>
                    </div>
                    <div class="form">
                        <div class='loginTitle'>
                            密&emsp;码&#8194;|&#8194;
                        </div>
                        <i-input :value.sync="value"  type="password" placeholder="请输入密码" ></i-input>

                    </div>
                </div>
                <div class="innerPass">
                    <p class="bstyle">
                        记住密码&#8194;<input  type="checkbox" value="记住密码">
                    </p>
                    <p class="cstyle">
                        <router-link to="">忘记密码</router-link>
                    </p>
                </div>
                <div class="inform">
                        <Button type="success" long @click="login()">登录</Button>
                        <br><br>
                        <Button type="error" long>注销</Button>
                        <router-link to='/register'>没有账号？马上注册</router-link>
                </div>
            
            </div>
        </div>
    </div>
     
</template>
<script>
import Head2 from '../components/Head2.vue'
import Head1 from '../components/Head1.vue'

    export default {
         data () {
            return {
                value: ''
            }
        },
        components:{
            Head2,Head1
        },
        mounted:{
            login(){
                
            }
        }
       
    }
</script>
<style >
    .login{
        width: 100%;
        height:700px;
        text-align: center;
    }
   
    .iform{
        width: 70%;
        height: 100%;
        margin: auto;
        background-color: azure;
        
    }
     h3{
        height: 175px;
        width: 100%;
        line-height: 175px;
        color: rgba(6, 32, 28, 0.562);
        font-size: 25px;
    }
   .loginabout {
        /* background: url(../assets/1.jpg); */
        width: 49%;
        height: 40%;
        float: left;
        background-size: 100% 100%;
      
    }
    .loginabout img{
        width: 94%;
        height: 100%;   
        margin: auto;
        }
    .loginform{
        width: 50%;
        height:40%;
        float: left;
    }
    .loginOne{
        width: 95%;
        height: 50%;
        margin: auto;

    }
    .form{
        width: 100%;
        height: 50%;
    }
   .loginTitle {
        width: 20%;
        height: 100%;
        font-size: 14px;
        line-height: 80px;
        float: left;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        color: rgba(48, 56, 50, 0.507)
    }
    .form .ivu-input-wrapper {
        display: inline-block;
        width: 75%;
        position: relative;
        vertical-align: middle;
        line-height: 80px;
        float: left;
    }
    .innerPass{
        width: 100%;
        height: 30px;
        
    }
    .bstyle{
        width: 50%;
        height: 100%;
        float: left;
        line-height: 30px;
    }
    .cstyle{
        width: 50%;
        height: 100%;
        float: right;
        line-height: 30px;
    }
    .inform {
        width: 95%;
        height: calc(100%-10px);
        text-align: center;
        margin: auto;
        margin-top: 20px;
    }
</style>