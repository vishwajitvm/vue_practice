<template>
  <div>
    <h1>Itrating array from propertys</h1>
    <div id="arraydata">
            <li v-for="item in technplogy" :key="item">
            {{ item }}
            </li>
    </div>
    <br> <br>
        <h1>Itrating arrays of Object from propertys</h1>
        <li v-for="itemdata in user" :key="itemdata">
        Name: {{ itemdata.name }} &nbsp;&nbsp;&nbsp;&nbsp; email: {{ itemdata.email }} &nbsp;&nbsp;&nbsp;&nbsp; phone: {{ itemdata.mobile }}
        </li>
  </div>
</template>

<script>
export default {
    name: 'ForLoop',
    data() {
        return{
            technplogy: ['javascript' , 'laravel' , 'Php' , 'Vue-js' , 'angular' , 'React js' , 'Mysql database'],
            //arrays of object
            user:[
               {
                 name: "Vishwajit VM",
                 email: "Vishwwajit@gmail.com",
                 mobile: 8920352117,
               },
               {
                 name: "Shivani",
                 email: "shivani@gmail.com",
                 mobile: 585475958,
               },
               {
                 name: "Manish",
                 email: "manish@gmail.com",
                 mobile: 715756854,
               },
               {
                 name: "palavi ",
                 email: "palavi@gmail.com",
                 mobile: 5858454512,
               },
            ]
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