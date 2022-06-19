<template>
  <div style="background:#262624;color:aliceblue;padding: 40px;">
    <h1> Event Management Practice </h1>
    <button v-on:click="CountData()" >Click me baby</button>
    <h3> {{ count }} </h3>
  </div>
</template>

<script>
export default {
  name: 'EventFunction2Practice',
  data() {
    return{
      count:0
    }
  },
  methods: {
    CountData() {
      return this.count = this.count+1
    }
  },
}
</script>


<style scoped>
  button{
    background: rgb(233, 58, 58);
    padding: 10px;
    color: azure;
  }
</style>