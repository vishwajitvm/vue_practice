<template>
  <div>
    <!-- <h2 class="otherclass" :class="{green:colorfull,err:true}">Hello world, class binding</h2> -->
        <h2 class="otherclass" :class="applyStyle">Hello world, class binding</h2>
    <button v-on:click="colorfull=!colorfull,fontSIze=!fontSIze" >Apply style</button>
  </div>
</template>
 
<script>
export default {
    name: 'ClassBinding',
    data() {
        return {
            colorfull: true,
            fontSIze: false
        }
    },
    computed:{
        applyStyle() {
            return{
                green:this.colorfull, //color change
                err:true,
                other:this.fontSIze, //font size controll here
            }
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
.green{
        background: green;
    }
    .err{
        color: red;
    }

    .other{
        font-size: 50px;
    }

    button{
        background: red;
        color: white;
        width: 200px;
        height: 50px;
        border-radius: 8%;
    }
    

</style>