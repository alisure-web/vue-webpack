<template>
  <div id="content">
    <my-button theme="theme-2" text="我6去" height="32px"
               width="64px" font-size="14px" @clickButton="myButtonClick"></my-button>
  </div>
</template>

<script>
  import Hello from './components/Hello'
  import myButton from './components/button.vue'

  export default {
    name: 'app',
    components: {
      myButton
    },
    methods: {
      myButtonClick: function () {
        alert("点击按钮");
        location.href = "http://www.alisure.xyz";
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
