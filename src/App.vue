<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <ImgLooking url="https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg"/>
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld.vue';
  import ImgLooking from './components/ImgLooking/index.vue';
  export default {
    name: 'App',
    data() {
      return {
      }
    },
    components: {
      HelloWorld,
      ImgLooking,
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
