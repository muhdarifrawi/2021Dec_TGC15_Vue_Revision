<template>
    <p :style="{color:textColor, fontSize:currentSize}" id="message">{{message}}</p>
    <button @click="changeColor">Change Color</button>
    <button @click="grow">Grow</button>
    <button @click="shrink">Shrink</button>
</template>
<script>
export default {
    data:function(){
        return{
            message:"This is a standard message",
            textColor:"red",
            currentSize: "32px"
        }
    },
    methods:{
        changeColor: function(){
            this.textColor = "green";
        },
        grow: function(){
            this.currentSize = parseInt(this.currentSize.slice(0,-2)) + 1 + "px";
        },
        shrink: function(){
            this.currentSize = parseInt(this.currentSize.slice(0,-2)) - 1 + "px";
        }
    }
}
</script>
<style>
</style>