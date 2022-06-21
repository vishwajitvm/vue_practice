<template>
  <div>
        <div id="userss">
        Name: {{ data.name }} <br>
        email: {{ data.email }} <br>
        phone: {{ data.mobile }} <br>  <br>
        <!-- <button v-on:click="getData()">Click me</button> -->
        <button v-on:click="getUserData(data.name,data.email , data.mobile)">Click me {{ data.name }} </button>

        </div>
  </div>
</template>

<script>
export default {
    name: 'ReuseChildComponent',
    props:{
        data:Object,
        getUserData:Function
    },
    // methods:{
    //     getData() {
    //         return alert(this.data.name)
    //     }
    // }
}
</script>

<style>
#userss{
    background: rgb(95, 43, 236);
    padding: 10px;
    border-bottom: 1px solid;
    margin-bottom: 20px;
}
</style>