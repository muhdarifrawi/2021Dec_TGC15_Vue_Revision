<template>
    <div>{{parseInt(number1) + parseInt(number2)}}</div>    
</template>
<script>
export default {
    name:"addBox",
    props:["number1","number2"]
}
</script>
<style>

</style>