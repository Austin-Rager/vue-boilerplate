<script setup>
  import { BaseTransitionPropsValidators, ref } from 'vue';
  let count = ref(0);
  let isActive = ref(true);
  let myList = ref(["Apples","Bananas","Oranges","Meat","Fish"]);

  function increment() {
    count.value++;
    console.log('count is now ' + count.value);

      }
</script>

<template>
  <div class="container">
    <h1>I am Austin Rager!</h1>
    <p>This is where I am trying to learn how to use vue.js!!</p>
    <button v-on:click="increment">Click me!</button>
    <p>Current count is: {{count}}</p>
    <p v-for="item in myList" :key="myList.id">This is what is in the list: {{myList.}}</p>
    <h3>I am going to try and learn a lot!</h3>
  </div>
</template>

<style scoped>
p {
  font-size: 20px;
  color: #333;
}

h1{
  background-color: aqua;
  border-radius: 3px;
  padding: 1rem;
}

button{
  padding: 8px;
  background-color: #11ff00;
}

a{
  text-decoration: none;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
</style>