<template>
  <div>
    hello, from Ref <br>

    <input type="text" ref="inputuserdata" /> <br> 
    <button v-on:click="getData">Click me</button>
  </div>
</template>

<script>
export default {
    name: 'RefComponents' ,
    methods:{
        getData() {
            this.$refs.inputuserdata.focus() ; //focus on defined [inputuserdata] input
            this.$refs.inputuserdata.style.color="red" ; //styling the text inside [inputuserdata]
            //get value of ref [inputuserdata]
            let valueofinput = this.$refs.inputuserdata.value;
            console.log(valueofinput);
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
        height: 35px;
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