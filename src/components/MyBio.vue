<template>
  <h1>Name: {{ name }}</h1>
  <h2>Age: {{ age }}</h2>
  <h2>Birthplace: {{ birthplace }}</h2>
  <h2>Current Location: {{ currentLocation }}</h2>
</template>

<script setup>
import { ref } from "vue";

defineProps({
  name: {
    type: String,
    default: "Cristina",
    required: true,
  },
  age: {
    type: Number,
    default: 35,
  },
  birthplace: {
    type: String,
    default: "Igualada",
  },
  currentLocation: {
    type: String,
    default: "Montbui",
  },
});
</script>

<style scoped></style>
