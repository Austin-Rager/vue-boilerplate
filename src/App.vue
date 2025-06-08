<script setup>
import { ref } from 'vue';

const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <div class="container">
    <p>Hello World!</p>
    <p>Welcome to your Vue.js app!</p>
    <p>Count: {{ count }}</p>
    <button @click="increment">Increment</button>
  </div>
</template>

<style scoped>
p {
  font-size: 20px;
  color: #333;
}
button {
  padding: 10px 20px;
  background-color: #42b983;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
button:hover {
  background-color: #35495e;
}
button:active {
  background-color: #2c3e50;
}
button:focus {
  outline: none;
}
button:focus-visible {
  outline: 2px solid #42b983;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
</style>