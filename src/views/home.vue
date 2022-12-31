<template>
  <div class="parent">
    <h1>我是首页</h1>
    <message-box :isShow="showBox" />
  </div>
</template>

<script>

import messageBox from '@/components/messageBox.vue'

export default {
  components:{
    messageBox
  },
  data(){
    return{
      showBox:false
    }
  }
}
</script>

<style scoped>
  .parent{
    max-width:1338px;
    position:relative;
  }
</style>