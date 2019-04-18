<template>
  <div class="head2">
    <div class="title1">
      <div class="tit"> 
          <div class='title'>农业咨询交流平台</div>
            <router-link to='/register'>注册</router-link>
            <router-link to='/login'>登录&#8194;|&#8194;</router-link>
        </div>   
    </div>
  </div>
</template>

<script>
export default {
  name: 'Head2',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 .head1{
    width: 100%;
    height: 80px;

 }

  .title1{
   width:100%;
   height: 30px;
   background-color: rgba(228, 227, 227, 0.5);    
  }
  .tit{
    width:95%;
    height: 100%;
    margin: auto;
    line-height: 30px;

  a{
      float: right;
      color:  #9ea7b4;
      font-size: 12px;
    }
  }
  .title{
    float: left;
    color:  #9ea7b4;
    font-size: 12px;
  }
  .one{
    float: left;
    line-height:40px;
  }
  .oneContent{
    float: left;
    height: 100%;
    font-size: 15px;
    text-align: center;
    margin: auto;
    line-height: 50px;
    a{
      color: cadetblue;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif
  
    }
   }
</style>
