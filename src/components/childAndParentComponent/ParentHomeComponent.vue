<template>
  <div>
    <childComponent  name="VishwaVM Child props" :user="user" :getData="getData"/>
  </div>
</template>

<script>
import childComponent from './childComponent.vue' 
export default {
    name: 'ParentHomeComponent',
    components:{
        childComponent
    },
    data() {
        return {
            user:{
                 name: "Vishwajit VM",
                 email: "Vishwwajit@gmail.com",
                 mobile: 8920352117,
               },
        }
    },
    methods: {
        getData() {
            alert( "hello world, from parent component")
        }
    },
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