<template>
  <div class="messageBox">
    <h1 class="messageBox-h1">绑定手机号</h1>
    <img src="../assets/img/cancel.png" alt="" class="messageBox-img">
    <div class="messageBox-bottom">
      <img src="../assets/img/mobile.png" alt="" class="messageBox-bottom-img img-top">
      <input type="text" placeholder="请输入手机号" class="messageBox-bottom-input">
      <button class="messageBox-bottom-code redText">获取验证码</button>
      <img src="../assets/img/code.png" alt="" class="messageBox-bottom-img img-bottom">
      <input type="text" placeholder="请输入验证码" class="messageBox-bottom-input">
      <button class="messageBox-bottom-btn">确认</button>
      <button class="messageBox-bottom-btn whiteBackground noBorder">没有收到验证码？<span class="redText">联系客服</span></button>
    </div>
  </div>
</template>

<script>
  export default {
    props:{
      isShow:{
        default:false,
        type:Boolean
      }
    }
  }
</script>

<style scoped>

  .img-top{
    top:8%;
  }
  .img-bottom{
    top:34%;
  }
  .messageBox-bottom-img{
    width:5%;
    position:absolute;
    /* top:2%; */
    left:12%;
    z-index: 1;
  }
  .messageBox-bottom-code{
    position:absolute;
    top:31%;
    left:65%;
    width:20%;
    z-index: 1;
    cursor: pointer;
    /* 行高必须写死 */
    line-height: 40px;
    border:none;
    background:none;
  }
  .messageBox-bottom-btn{
    /* 行高必须写死 */
    line-height: 40px; 
    width:100%;
    margin:4% 0;
    cursor: pointer;
  }
  .messageBox-bottom-input{
    width:100%;
    /* 行高必须要写死 */
    line-height: 40px;
    margin:4% 0;
    padding:0 10%;
  }
  .messageBox-bottom{
    border:1px solid red;
    padding:0 10%;
  }
  .messageBox-img{
    width:5%;
    position:absolute;
    left:90%;
    top:5%;
    cursor: pointer;
  }
  .messageBox-h1{
    text-align: center;
    color:white;
    background:red;
    border-top-left-radius: 4%;
    border-top-right-radius: 4%;
  }
  .messageBox{
    /* 子元素上下左右在页面句子的终极方法 */
    position:fixed;
    top:0;
    left:0;
    right:0;
    bottom:0;
    margin:auto auto auto auto;
    width:30%;
    height:300px;
    background:white;
  }
  .whiteBackground{
    background:white;
  }
  .redText{
    color:red;
  }
  .whiteText{
    color:white;
  }
  .noBorder{
    border:none;
  }
</style>