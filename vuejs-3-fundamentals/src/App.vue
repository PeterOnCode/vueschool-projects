<script setup lang="ts">
import {ref} from "vue";

const header = ref("Shopping list App")
</script>

<template>
  <h1>{{ header || "Welcome" }}</h1>
  <input v-model="header">
</template>

<style scoped>

</style>
