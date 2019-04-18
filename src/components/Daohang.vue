
<template>
    <div class="Daohang">
        <!-- <Head1/> -->
        <div id="nav">
            <router-link to="/">首页</router-link> |
            <router-link to="/plaza">广场</router-link>|
            <router-link to="/chat">闲聊</router-link>|
            <router-link to="/topsNews">热点</router-link>|
            <router-link to="/information">资讯</router-link>|
            <router-link to="/plant">政策</router-link>|
            <router-link to="/ecommerce">新技术</router-link>|
            <router-link to="/details">新技术</router-link>|
            <span> 现在是北京时间:{{time}}</span>
            <!-- <button @click='Time()'>11</button> -->
        </div>
        <!-- <Foot1/> -->
    </div>
</template>
<script>
// @ is an alias to /src
// import Foot1 from '@/components/Foot1.vue'//引入路由部分(公用组件)
// import Head1 from '@/components/Head1.vue'//引入路由部分(公用组件)
//引入外部js
import {getTime} from '../js/IntoVue.js'

export default {
    components: {//引入路由部分(公用组件)
        // Foot1,
        // Head1
    },
    data(){
        return{
            time:''
        }
    },
    mounted:function(){
        this.Time();
    },
    methods: {
        Time(){
            this.time=getTime();
             console.log(this.time)

        },
        
    },
}
</script>
<style lang="scss">
    .Daohang {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }
    #nav {
        width: 100%;
        background-color: cadetblue;
        height: 50px;
        line-height: 50px;
        a {
            font-weight: bold;
            color: #2c3e50;
            font-size: 20px;
            // float: left;
            // background-color: rgba(181, 248, 250,0.4);
            &.router-link-exact-active {
            color: #e3f5ed;
            font-size: 21px;

            }
        }
    }
</style>
    