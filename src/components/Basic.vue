<template>
    <div>
        <img src="../assets/logo.png" />
        <h1 class="title">Hello world~</h1>
        <p>{{message}}</p>
        <p>{{message2}}</p>
        <button @click="changeMessage">Change thy message</button><br>
        <!-- @click is much easier to type than v-on:click but both functions the same way -->
        <button v-on:click="changeMessage2">Change another one</button>
    </div>
</template>

<script>
export default {
    name: "Basic",
    data: function(){
        return {
            "message":"Welcome to Vue application.",
            "message2":"Tide goes in ..."
        }
    },
    methods:{
        changeMessage: function(){
            this.message = "Hope you enjoyed your stay!";
        },
        changeMessage2: function(){
            this.message2 = "... Tide goes out";
        }
    }
}
</script>

<style>
.title{
    font-family: Verdana;
}
</style>