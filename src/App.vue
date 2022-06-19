<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Vishwajit Vm"/> -->
  <!-- <InterPolComponent></InterPolComponent> -->
  <!-- <MethodsWithParam></MethodsWithParam> -->
  <!-- <EventFunctions /> -->
  <!-- <EventFunction2Practice /> -->
  <!-- <TwoWayBinding></TwoWayBinding> -->
  <GetInputValues></GetInputValues>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import InterPolComponent from './components/InterPolComponent.vue'
// import MethodsWithParam from './components/MethodsWithParam.vue'
// import EventFunctions from './components/EventFunctions.vue'
// import EventFunction2Practice from './components/EventFunction2Practice.vue'
// import TwoWayBinding from './components/TwoWayBinding.vue'
import GetInputValues from './components/GetInputValues.vue' 

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // InterPolComponent,
    // MethodsWithParam,
    // EventFunctions,
    // EventFunction2Practice,
    // TwoWayBinding,
    GetInputValues
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
