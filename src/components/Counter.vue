<template>
    <h4>{{counterValue}}</h4>
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
            counterValue:0
        }
    },
    methods:{
        add:function(){
            this.counterValue = this.counterValue + 1;
        },
        subtract:function(){
            this.counterValue = this.counterValue - 1;
        }
    }
}
</script>
<style>

</style>