<template>
    <h1>{{message}}</h1>
    <button @click="greet">Greet za worl</button>
    <button @click="farewell">Goodbye worl</button>
    <button @click="goodnight">Goodnight worl</button>
</template>

<script>
export default {
    data:function(){
        return{
            "message": "Welcome to the instance."
        }
    },
    methods:{
        greet:function(){
                this.message = "HALLO WORLD~!!!"
        },
        farewell:function(){
            this.message = "FAREWELL WORLD~!!!"
        },
        goodnight: function(){
            this.message = "GOODNIGHT WORLD~!!!"
        }
    }
}
</script>

<style>

</style>