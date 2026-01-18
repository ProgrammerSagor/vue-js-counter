<script setup>

import { ref } from 'vue';

const count = ref(0);
const increment = () => {
    count.value += 1;
}

const decrement = () => {
    count.value -= 1;
}
</script>



<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gradient-to-r from-purple-500 to-pink-500 font-sans">
    <h1 class="text-4xl font-bold text-white mb-8 drop-shadow-lg">Counter Display</h1>

    <div class="bg-white rounded-xl shadow-lg p-8 flex flex-col items-center gap-6">
      <h2 class="text-6xl font-extrabold text-gray-800">{{ count }}</h2>

      <div class="flex gap-4">
        <button @click="increment" class="px-6 py-3 bg-green-500 text-white font-bold rounded-lg shadow hover:bg-green-600 transition">
          +
        </button>
        <button @click="decrement" class="px-6 py-3 bg-red-500 text-white font-bold rounded-lg shadow hover:bg-red-600 transition">
          -
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped></style>



