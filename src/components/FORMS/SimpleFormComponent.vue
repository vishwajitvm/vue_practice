<template>
  <div>
    <h2> SIMPLE FORM  </h2>
  </div>
</template>

<script>
export default {
    name: 'SimpleFormComponent' ,

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