<template>
    <div id="box"></div>
</template>

<script>
export default {
    data: function(){
        return {
            number: Math.floor(Math.random() * 100 + 1)
        }
    }
}
</script>

<style>
#box{
    border: 2px solid black;
    height: 30px;
    width:30px;
}
</style>