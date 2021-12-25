<template>
  <div
    id="box"
    v-bind:style="{
      backgroundColor: color,
    }"
  ></div>
</template>
<script>
export default {
  data: function () {
    let theColor = ["red", "blue", "green"];
    return {
      color: theColor[Math.floor(Math.random()*theColor.length)],
    };
  },
};
</script>
<style scoped>
#box {
  width: 50px;
  height: 50px;
  border: 1px solid black;
}
</style>