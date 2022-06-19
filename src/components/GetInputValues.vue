<template>
  <div>
    <h1>Get Values From Input Field</h1>
    <br>
    <input type="text" placeholder="Enter email" v-model="email" /> <br>
    <input type="text"  placeholder="Enter password" v-model="password" /> <br>
    <button type="button" v-on:click="getData()">Get Values</button>
        <h3>email: {{email}} <br> password: {{password}}</h3>
  </div>
</template>

<script>
export default {
    name: 'GetInputValues',
    //property
    data() {
        return {
            email:null,
            password:null
        }
    },
    //function
    methods: {
        getData() {
            let emails = this.email;
            let passwords = this.password;
            return console.log("email: " ,emails , "Password:" , passwords) ;
        }
    },
}

</script>

<style scoped>
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
        width: 400px;
        height: 30px;
        margin-top: 8px;
        border-radius: 6%;
        padding-left: 20px;
    }
    input:focus{
        background: white;
    }
</style>