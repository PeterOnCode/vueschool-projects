<script setup lang="ts">
import {reactive, ref} from "vue";

const header = ref("Shopping list App")
const items = reactive([
  {id:1,label:"10 party hats"},
  {id:2,label:"2 board games"},
  {id:3,label:"20 cups"}
])
</script>

<template>
  <h1>{{ header || "Welcome" }}</h1>
  <ul>
    <li v-for="item in items" :key="item.id">{{ item.label }}</li>
    <li>---</li>
    <li v-for="{id,label} in items" :key="id">{{ label }}</li>
    <li>---</li>
    <li v-for="(item, index) in items" :key="index">{{index}}: {{ item.label }}</li>
  </ul>
</template>

<style scoped>

</style>
