<template>
    <div>
        <h4>FuctionCalling : {{ getNameData("Durgesh dm") }}</h4>
        <h5> object fucntion return here: {{ getData().name }} </h5>
        <h4> object maile here: {{ getData().email }} </h4>
        <h3> My phone number: {{ getData().phonenumber }} </h3>
        <br>
        <div id="dmd">
            <h1>DURGESH DATA HERE</h1>
        <h3> Name: {{ DurgeshData().name }} </h3>
        <h3> Email: {{ DurgeshData().email }} </h3>
        <h3> Phone: {{ DurgeshData().phon }} </h3>
        <h3> Address: {{ DurgeshData().address }} </h3>

        </div>
    </div>
</template>

<script>
export default {
    name: 'MethodsWithParam',
    methods:{
        getNameData(a) {
            return a ;
        },
        getData() {
            return {
                name: "Vishwajitvm object" ,
                email: "vishwajitm@gmail.com object",
                phonenumber: 8920352115
            }
        },
        DurgeshData() {
            return {
                name: "durgesh mall" ,
                email: this.getData().email, //uses this method to fetch the getData email in this function
                phon: 123458285,
                address: "new delhi"
            }
        }
    }
}
</script>

<style scoped>
#dmd h1{
    color: red;
}
#dmd h3{
    color: blueviolet;
    
}
</style>