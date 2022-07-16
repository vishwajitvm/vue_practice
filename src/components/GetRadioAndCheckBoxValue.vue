<template>
  <div>
    <h1>Get Checkboxes  Values</h1>
    <br>
    <h1>Technology</h1>
    <input type="checkbox" value="Java"  id="java"  v-model="technology"/>    <label for="java">Java</label>  <br>
    <input type="checkbox" value="php" id="php" v-model="technology"/>    <label for="php">php</label>  <br>
    <input type="checkbox" value="ruby" id="ruby" v-model="technology"/>    <label for="ruby">ruby</label>  <br>
    <input type="checkbox" value="Vue" id="Vue" v-model="technology"/>    <label for="Vue">Vue</label>  <br>
    <input type="checkbox" value="Node" id="Node" v-model="technology"/>    <label for="Node">Node</label>  <br> <br> <br>

<h3> Check Box Selected technology: {{ technology }} </h3>
<br><br>

    <h1>Get Radio Data   Values</h1>
    <h3> Who I am? </h3>
    <input type="radio" value="student" id="student" v-model="technologyRadio"/>    <label for="student">student</label>  <br> 
    <input type="radio" value="Teacher" id="Teacher" v-model="technologyRadio"/>    <label for="Teacher">Teacher</label>  <br> 
    <input type="radio" value="Principal" id="Principal" v-model="technologyRadio"/>    <label for="Principal">Principal</label>  <br> 
    <input type="radio" value="Caption" id="Caption" v-model="technologyRadio"/>    <label for="Caption">Caption</label>  <br> <br> <br> 


    <h3> Check Box Selected technology: {{ technologyRadio }} </h3>



  </div>
</template>

<script>
export default {
    name: 'GetRadioAndCheckBoxValue',
    data() {
      return {
        technology: [],
        technologyRadio:[]
      }
    }
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