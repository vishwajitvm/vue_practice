<template>
  <div>
    <h2> SIMPLE FORM  </h2>
        <form action="">
            <input type="text" placeholder="Enter Name" autocomplete="on" v-model="formData.username" /> <br> 
            <input type="email" placeholder="Enter Email"  autocomplete="on"  v-model="formData.useremail" /> <br> 
            <input type="password" autocomplete="on"  placeholder="Enter Password" v-model="formData.userpassword" />  <br>
            <button v-on:click="login" type="button">Click me</button>
        </form>

        {{ formData }}

  </div>
</template>

<script>
export default {
    name: 'SimpleFormComponent' ,
    data() {
        return{
            formData:{
                username:'',
                useremail:'',
                userpassword:''
            }
        }
    },
    methods:{
        login() {
            console.warn("login data", this.formData)
        }
    }

}
</script>

<style scoped>
    *{
        color:azure
    }
    button{
        color: white;
        width: 430px;
        height: 50px;
        margin-top: 10px;
        background: rgba(0, 128, 0, 0.555);
    }
    
    button:hover{
        color: white;
        background: green;
    }
    input{
        background: rgb(235, 220, 220);
        color: black;
        width: 400px;
        height: 35px;
        margin-top: 8px;
        border-radius: 6%;
        padding-left: 20px;
    }
    input:focus{
        background: white;
    }

</style>