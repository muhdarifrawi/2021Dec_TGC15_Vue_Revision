<template>
    <h4 :style="{color:currentColor}" @change="checkColor">{{counterValue}}</h4>
    <p v-if="counterValue%2 == 0">Even Number</p>
    <p v-else-if="counterValue%2 != 0">Odd Number</p>
    <p v-else>Something went wrong</p>
    <button @click="add">Add</button>
    <button @click="subtract">Subtract</button> 
</template>
<script>
export default {
    data:function(){
        return{
            counterValue:0,
            currentColor:"black"
        }
    },
    methods:{
        add:function(){
            this.counterValue = this.counterValue + 1;
        },
        subtract:function(){
            this.counterValue = this.counterValue - 1;
        },
        checkColor:function(){
            if (this.counterValue%2 == 0){
                this.currentColor = "blue";
            }
            else{
                this.currentColor = "red";
            }
        }
    }
}
</script>
<style>

</style>