<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <ButtonComp></ButtonComp>

    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import ButtonComp from "./components/ButtonComp";


export default {
  name: 'app',
  components: {
    HelloWorld,
    ButtonComp,
  
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
