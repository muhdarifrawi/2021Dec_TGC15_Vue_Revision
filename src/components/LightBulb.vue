<template>
  <div>
    <div v-if="switchedOn=='true'">
        <img src="../assets/bulb-on.jpeg" />
    </div>
    <div v-else-if="switchedOn=='false'">
        <img src="../assets/bulb-off.webp" />
    </div>
    <div v-else><p>Unexpected Error.</p></div>   
    
    
  </div>
</template>

<script>
export default {
  name: "LightBulb",
  props:['switchedOn']
};
</script>

<style scoped>
img {
  width: 200px;
}
</style>