<template>
  <div>
    <h1> If else Statment </h1>
    <div id="ifelsedata">
        <h1 v-if="show"> If Condition is true </h1>
        <h1 v-else> Else Condition is true </h1>
        <button v-on:click="show=!show">Click Me</button>
    </div>
  </div>
</template>

<script>
export default {
    name: 'IfElseConditions',
    data() {
        return {
            show: false
        }
    }
}
</script>

<style>
    *{
        color:azure
    }
        button{
        color: black;
        width: 430px;
        height: 30px;
        margin-top: 10px;
        background: green;
    }
    input{
        background: rgb(235, 220, 220);
        color: black;
        width: 80px;
        height: 25px;
        margin-top: 8px;
        border-radius: 6%;
        padding-left: 20px;
    }
    input:focus{
        background: white;
    }
    

</style>