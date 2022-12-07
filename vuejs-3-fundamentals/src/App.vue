<script setup lang="ts">
import {ref} from "vue";

const header = ref("Vue is ready to party!")
</script>

<template>
  <h1>Header text: {{ header }}</h1>
  <input v-model="header">
</template>

<style scoped>

</style>
