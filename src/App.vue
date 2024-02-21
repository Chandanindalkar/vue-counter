<!-- the setup inside <script> is a compile-time syntactic sugar for using Composition API inside -->

<script setup>
  import { ref } from "vue";

  const count = ref(5);
</script>

<template>
  <main>
    <div>
      <h2>
        The current count is:
      </h2>
      <h1>{{ count }}</h1>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </main>
</template>

<!-- the scoped inside <styles> is to make it available only locally -->
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
