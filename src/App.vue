<template>
  <Basic/>
  <Alert message="Danger danger" bgColor="salmon" />
  <Alert message="This is a test" textSize="32px" bgColor="orange" />
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
  <RandomBox></RandomBox>
  <SayGreetings></SayGreetings>
  <ColoredBox></ColoredBox>
  <ColoredBox></ColoredBox>
  <ColoredBox></ColoredBox>
  <Counter></Counter>
  <Dice></Dice>
  <ChangeText></ChangeText>
  <LightBulb switchedOn="false" />
  <AddBox number1="11" number2="12" />
</template>

<script>
import Basic from './components/Basic.vue'
import RandomBox from './components/RandomBox.vue'
import SayGreetings from './components/SayGreetings.vue'
import ColoredBox from './components/ColoredBox.vue'
import Counter from './components/Counter.vue'
import Dice from './components/Dice.vue'
import ChangeText from './components/ChangeText.vue'
import Alert from './components/Alert.vue'
import LightBulb from'./components/LightBulb.vue'
import AddBox from './components/AddBox.vue'

export default {
  name: 'App',
  components: {
    Basic,
    RandomBox,
    SayGreetings,
    ColoredBox,
    Counter,
    Dice,
    ChangeText,
    Alert,
    LightBulb,
    AddBox
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
