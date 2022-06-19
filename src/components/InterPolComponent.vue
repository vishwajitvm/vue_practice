<template>
    <div>
        <h1> {{email}} </h1>
        <h1> {{mobile}} </h1>
        <h1> {{getName()}} </h1>
        <h1> {{getName2Parameter('vishwajit is legend')}} </h1>

    </div>
</template>

<script>
    export default {
        name: 'InterPolComponent',
        data() {
            return {
                email: 'Vishwajit@gmail.com',
                mobile: 1234567890 ,
                getName: function() {
                    return "Vishwajit"
                },
                getName2Parameter: function (abc) {
                    return abc;
                }
            
            }
        }
    }
</script>