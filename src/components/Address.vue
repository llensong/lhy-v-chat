<template>
    <div class='Address'>
        <div class=AddContents>
            <div class="AddCont"><router-link to="/">首页</router-link></div>
            <div class="AddCont">&#8194;/&#8194;PageName</div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
        }
    },
    mounted:{
        
    },
    methods:{
       
    }
    
}
</script>
<style lang="scss">
    .Address{
        width: 100%;
        height: 30px;
        background-color: cadetblue;
    }
    .AddContents{
        width: 95%;
        height: 100%;
        color: #e3f5ed;
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-size: 12px;
        margin: auto;
        line-height: 30px;
    }
    .AddCont{
        float: left;
         a {
            font-weight: bold;
            color: #e3f5ed;           
        }
    }
</style>