<template>
    <div class="alert" v-bind:style="{backgroundColor:bgColor, fontSize: textSize}">{{message}}</div>
</template>
<script>
export default {
    name:"Alert",
    props:["message","bgColor", "textSize"]
}
</script>
<style>
.alert{
    background-color:mistyrose;
    font-style:12px;
}
</style>