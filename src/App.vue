<script setup>
import { ref } from "vue";
const count = ref(0);

const addNumber = () => {
  count.value = count.value + 1;
}

const subtractNumber = () => {
  count.value = count.value - 1;
}

</script>

<template>
  <main>
    <div>
      <h4>The current count is ...</h4>
      <h1>{{ count }}</h1>
      <button @click="subtractNumber">-</button>
      <button @click="addNumber">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>