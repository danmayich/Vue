<script setup>
  import {ref} from "vue"

  const count = ref(0);

</script>

<template>
  <main>
    <div>
      <h4>
      The current count is ...
      </h4>
      <h1>{{ count }}</h1>
      <Button @click="count--">-</Button>
      <Button @click="count++">+</Button>
    </div>
  </main>
</template>

<style scoped>
  main {
    background-color: rgb(39, 39, 191);
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