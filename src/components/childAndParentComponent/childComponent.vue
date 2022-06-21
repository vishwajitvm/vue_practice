<template>
  <div>
    Simple Props  {{ name }}

    <br> <br>
    <h1>Calling an object from parents using props</h1>
    <h4> {{ user.email }} </h4>
    <h4> {{ user.mobile }} </h4>


        <br> <br>
    <h1>Calling an Methods from parents to Child using props</h1>

    <button v-on:click="getData">Calling data from parent component in console</button>
  </div>
</template>

<script>
export default {
    name: 'childComponent',
    //importing props from parents to child here 
    props:{
        name:String,
        user:Object,
        getData:Function
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