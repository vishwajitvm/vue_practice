<template>
  <div>
    <h1> Learn to Reuse Component </h1>
    <h2> Printing arrays object value at Child  </h2>
    <li v-for="item in usersData" :key="item" >
        <!-- Name: {{ item.name }} <br>
        email: {{ item.email }} <br>
        phone: {{ item.mobile }} <br>  <br> -->

        <ReuseChildComponent :data="item" :getUserData="getUserData"/>

    </li>
    <!-- <ReuseChildComponent /> -->
  </div>
</template>

<script>
import ReuseChildComponent from './ReuseChildComponent.vue'
export default {
    name: 'ReuseParentCompo',
    components:{
        ReuseChildComponent
    },
    methods:{
        getUserData(username,useremail , usermobile) {
            return alert(username + " <br> "+ useremail + " <br> "+ usermobile)
        }
    },
    //Property [define some array to use it]
    data() {
        return {
            //arrays of object
            usersData:[
               {
                 name: "Vishwajit VM",
                 email: "Vishwwajit@gmail.com",
                 mobile: 8920352117,
               },//1
               {
                 name: "Shivani",
                 email: "shivani@gmail.com",
                 mobile: 585475958,
               },//2
               {
                 name: "Manish",
                 email: "manish@gmail.com",
                 mobile: 715756854,
               },//3
               {
                 name: "palavi ",
                 email: "palavi@gmail.com",
                 mobile: 5858454512,
               },//4
            ]//array end
        }//return end
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
    li{
        list-style: none;
    }
    

</style>