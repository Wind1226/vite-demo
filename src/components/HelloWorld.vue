<script setup>
import { ref } from 'vue'
defineProps({
  msg: String
})

const data = ref('121');
</script>

<template>
  <h1>{{ msg }}</h1>

  <input type="button" :value="`click me ${data}`" @click="data += 1" />
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
