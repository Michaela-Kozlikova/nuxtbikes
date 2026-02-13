<template>
  <button @click="count++">Increment {{ count }}</button>
</template>

<style>
button { 
  color: red}
</style>

<script setup>
import { ref } from "vue";
const count = ref(5);
</script>
