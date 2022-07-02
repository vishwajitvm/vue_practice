<template>
  <div>
    hello
    <ChildClass :getChildDataNamess="getChildDataName" />
    </div>
</template>

<script>
import ChildClass from './ChildClass.vue'
export default {
    name: 'ParentClass' ,
    components:{
        ChildClass
    },
    //we need to send method and pass an parrameter to get that data in parant
    methods: {
        getChildDataName(name) {
            alert(name) ;
        },
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