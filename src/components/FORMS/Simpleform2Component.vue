<template>
  <div>
    <h2> SIMPLE FORM 2  </h2>
            {{ formData }}

        <form action="">
            <input type="text" placeholder="Enter Name" autocomplete="on" v-model="formData.username" /> <br> 
            <input type="email" placeholder="Enter Email"  autocomplete="on"  v-model="formData.useremail" /> <br> 
            <input type="password" autocomplete="on"  placeholder="Enter Password" v-model="formData.userpassword" />  <br>
            <!--select--->
            <select v-model="formData.country"   id="selettoption">
                <option >India</option>
                <option>Brazil</option>
                <option>America</option>
                <option>Japan</option>
                <option>South Korea</option>
            </select> <br/>
            <!--checkbox -->
            <div>
            <input type="checkbox" value="java" class="inputcheckbox" v-model="formData.technology" name="java" id="java"> 
            <label for="java" class="checkboxlable">Java</label> <br>
            </div>

            <div>
            <input type="checkbox" value="php" class="inputcheckbox" v-model="formData.technology" name="java" id="php"> 
            <label for="php" class="checkboxlable"> php </label> <br>
            </div>

            <div>
            <input type="checkbox" value="vue" class="inputcheckbox" v-model="formData.technology" name="java" id="vue"> 
            <label for="vue" class="checkboxlable"> vue</label> <br>
            </div>
            <!--radio-->
            <div>
            <input type="radio" value="male" class="inputcheckbox" v-model="formData.gender" name="java" id="java"> 
            <label for="java" class="checkboxlable"> &nbsp;&nbsp; Male</label> <br>
            </div>

            <div>
            <input type="radio" value="femele" class="inputcheckbox" v-model="formData.gender" name="java" id="php"> 
            <label for="php" class="checkboxlable">Female</label> <br>
            </div>

            <div>
            <input type="radio" value="other" class="inputcheckbox" v-model="formData.gender" name="java" id="vue"> 
            <label for="vue" class="checkboxlable"> Other</label> <br>
            </div>

            <!--end-->
            <button v-on:click="login" type="button">Click me</button>
        </form>


  </div>
</template>

<script>
export default {
    name: 'Simpleform2Component' ,
    data() {
        return{
            formData:{
                username:'',
                useremail:'',
                userpassword:'',
                country:'',
                technology:[] ,
                gender:''
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
        #selettoption{
                /* background: rgb(235, 220, 220); */
        color: black;
        width: 420px;
        height: 35px;
        margin-top: 8px;
        /* border-radius: 2%; */
        padding-left: 20px;
        background: rgb(21, 200, 223);
        font-size: 20px;
    }
    input:focus{
        background: white;
    }
    /* checkbox */
        .radioinp input{
        background: rgb(235, 220, 220);
        color: black;
        width: 80px;
        height: 25px;
        margin-top: 8px;
        border-radius: 6%;
        padding-left: 20px;
    }
    .radioinp input:focus{
        background: white;
    }

    .inputcheckbox{
        margin-left: -400px !important;
    }

    .checkboxlable{
        font-size: 30px;
        margin-left: -90px !important;

    }
    


</style>