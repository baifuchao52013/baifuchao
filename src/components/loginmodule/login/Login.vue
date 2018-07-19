<template>
  <div class="module-login" v-if="showLogin">
    <login-box v-bind:title="title"></login-box>
  </div>
</template>

<script>
  import LoginBox from './LoginBox'
    export default {
        name: "login",
      components: {LoginBox},
      data(){
          return{
            title:"中国湿地",
            showLogin:true
          }
      }
    }
</script>

<style scoped>
    .module-login{
      position: absolute;
      top: 30%;
      right: 15%;
    }
</style>
