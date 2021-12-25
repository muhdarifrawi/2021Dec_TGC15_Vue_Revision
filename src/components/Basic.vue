<template>
    <div>
        <img src="../assets/logo.png" />
        <h1 class="title">Hello world~</h1>
        <p>{{message}}</p>
        <p>{{message2}}</p>
        <button @click="changeMessage">Change thy message</button><br>
        <!-- @click is much easier to type than v-on:click but both functions the same way -->
        <button v-on:click="changeMessage2">Change another one</button><br><br>
        <button @click="toggleLight">Toggle Light</button>
        <div class="light" v-if="this.light==true">
            Lights On
        </div>
        <div class="light" v-else>
            Lights Off
        </div>
    </div>
</template>

<script>
export default {
    name: "Basic",
    data: function(){
        return {
            message:"Welcome to Vue application.",
            message2:"Tide goes in ...",
            light:false
        }
    },
    methods:{
        changeMessage: function(){
            this.message = "Hope you enjoyed your stay!";
        },
        changeMessage2: function(){
            this.message2 = "... Tide goes out";
        },
        toggleLight: function(){
            this.light = !this.light;
        }
    }
}
</script>

<style>
.title{
    font-family: Verdana;
}
</style>