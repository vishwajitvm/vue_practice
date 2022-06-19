<template>
  <div style="background:black;color:aliceblue;padding: 40px;">
    <h1>Vue Event Management</h1>
    <button v-on:click="getData('button 1clicked')">Click Me</button> &nbsp; <!--  on Click click -->
        <button v-on:dblclick="getData('button 2 clicked')">Click Me</button> <!--  duble click --> 
        <br> <br>
        <button v-on:click="getCountNumber()">Click to Count CLick</button>
        <h2> {{count}} </h2>

  </div>
</template>

<script>

export default {
    name: 'EventFunctions',
    data() {
        return {
            count:0
        }
    },
    methods: {
        getData(data) {
            alert(data) ;
        },
        getCountNumber() {
            this.count = this.count+1;
        }
    }

    
}
</script>

<style scoped>
button{
    background: green;
    padding: 12px 10px;
    color: azure;

}
</style>