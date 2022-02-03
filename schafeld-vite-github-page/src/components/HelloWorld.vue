<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>

  <h1>{{ msg }}</h1>

  <p>
    My proper home page is:
    <a href="https://www.schafeld.com/" target="_blank">www.schafeld.com</a>
  </p>

  <p>
    Here's something to play with:
  </p>

  <button type="button" @click="count++">You clicked me: {{ count }} times.</button>

  <p v-if="count > 4">
    Naughty, naughty 😈
  </p>

</template>

<style scoped>
a {
  color: #44b436;
}
</style>
