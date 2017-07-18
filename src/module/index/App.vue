<template>
  <div id="content">
    <a href="./about.html">about</a>
    <img src="../../assets/logo.png">
    <my-button theme="theme-2" text="我688去" height="32px"
               width="64px" font-size="14px" @clickButton="myButtonClick"></my-button>
  </div>
</template>

<script>
  import myButton from '../../components/common/button.vue'

  export default {
    name: 'app',
    components: {
      myButton
    },
    methods: {
      myButtonClick: function () {
        alert("点击按钮");
        location.href = "./home.html";
      }
    }
  }
</script>

<style>
  #content {
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
