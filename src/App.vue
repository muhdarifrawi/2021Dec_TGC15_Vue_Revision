<template>
  <Basic/>
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
  <SayGreetings></SayGreetings>
  <ColoredBox></ColoredBox>
  <ColoredBox></ColoredBox>
  <ColoredBox></ColoredBox>
  <Counter></Counter>
</template>

<script>
import Basic from './components/Basic.vue'
import RandomBox from './components/RandomBox.vue'
import SayGreetings from './components/SayGreetings.vue'
import ColoredBox from './components/ColoredBox.vue'
import Counter from './components/Counter.vue'

export default {
  name: 'App',
  components: {
    Basic,
    RandomBox,
    SayGreetings,
    ColoredBox,
    Counter
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
