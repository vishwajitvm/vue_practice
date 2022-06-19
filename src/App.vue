<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Vishwajit Vm"/>
  <InterPolComponent></InterPolComponent>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import InterPolComponent from './components/InterPolComponent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    InterPolComponent
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
