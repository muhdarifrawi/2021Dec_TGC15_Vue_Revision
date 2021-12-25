<template>
  <br /><br />
  <p>{{ message }}<span v-if="message%2 == 0">!</span></p>
  <button @click="rollDice">Roll Dice</button>
</template>
<script>
export default {
  data: function(){
    return {
          message: "Press 'Roll Dice' to begin."
    }
  }
,
  methods: {
      rollDice: function(){
          this.message = Math.floor(Math.random()*6 + 1)
      }
  }
};
</script>
<style>
</style>