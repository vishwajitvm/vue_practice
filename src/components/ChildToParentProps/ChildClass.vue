<template>
  <div>
    <h3> Hello world   </h3>
    <button v-on:click="getChildDataNamess(ChildName)">Click to get data</button>
  </div>
</template>

<script>
export default {
    name: 'ChildClass',
    data() {
        return{
            ChildName: "Child data from child component"
        }
    } ,
    Props:{
        getChildDataNamess: Function
    }
}

</script>

<style>

</style>