<template>
  <div>
    <p> <span style="font-weight: bold;">Two way binding:</span> The v-model directive updates the template whenever the model changes and updates data model whenever the template changes. </p>
    <h2>Example: show changes in Model(script or js part) and replicate data in view vice-versa</h2> <br>

    <label for="datadata">Change value</label>
    <input type="text" id="datadata" v-model="count"> <br>
    <h2> {{ count }} </h2>
  </div>
</template>

<script>
export default {
    name:'TwoWayBinding.vue',
    //property
    data() {
        return {
            count:0
        }
    }
}
</script>

<style>
input{
    padding: 10px 100px 10px 8px;
}
label{
    margin-right: 20px;
}
</style>