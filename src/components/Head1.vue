<template>
    <div class="title2"> 
      <div class="title2one" style="width:70%;height:80px">
        <div class="oneContent">
          <img src='../assets/2019/111.jpg' alt="">
        </div>
        <div class="oneContent">
          <router-link to="/">
          农交网 |
          
          </router-link>
            <span>
              农业咨询交流平台
            </span>
          
        </div>
      </div >
      <div class="title2one" style="width:30%;height:80px;">
        <Input search  placeholder="请输入关键词" />
      </div>
     
    </div>  
    
</template>

<script>
export default {
  name: 'Head1',
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
 .title2{
   width:80%;
   height: 80px;
   margin: auto;
   img {
    /* border-style: none; */
      // line-height:80px; 
      height: 60%;
      width: 57px;
      // margin: auto;
      margin-top: 17px;
    } 
  }

  
  .title2one{
    float: left;
    line-height:80px;
  }
  .oneContent{
    float: left;
    height: 100%;
    font-size: 15px;
    text-align: center;
    margin: auto;
    line-height: 80px;
    a{
      color: cadetblue;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      font-size: 25px;
      font-weight: bold;

    }
    span{
      color:  rgba(141, 140, 140, 0.795);
      font-size: 15px;
    }
   }
</style>
