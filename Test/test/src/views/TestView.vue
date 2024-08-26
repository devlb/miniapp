
<template>
    <div class="about">
      <h1>测试页面啊</h1>
      <button  @click="test">button1</button>
      <div>{{info}}</div>
    </div>
</template>
  
<script>
  export default {
    data() {
      return {
        info: "啊啊"
      };
    },
    methods: {
      test() {
        console.log("测试");
        this.info = window.Telegram.WebApp.version
      },
    },
  };


</script>

  <style>
  @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  }
  </style>
  