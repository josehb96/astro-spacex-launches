<script lang="ts" setup>
import { ref } from 'vue';

const count = ref(0);

function increment() {
  count.value++;
}

function decrement() {
  count.value--;
}

</script>

<template>
  <div>
    <p>{{ count }}</p>
    <button class="border px-4 py-2 text-xl" @click="increment">+</button>
    <button class="border px-4 py-2 text-xl" @click="decrement">-</button>
  </div>
</template>