<template>
  <Basic/>
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
</template>

<script>
import Basic from './components/Basic.vue'
import RandomBox from './components/RandomBox.vue'

export default {
  name: 'App',
  components: {
    Basic,
    RandomBox
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
