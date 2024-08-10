<script setup lang="ts">
import {  ref } from 'vue'

const counter = ref(0)

function handleAdd() {
  counter.value += 1
}
</script>

<template>
  <div>
    {{ counter }}

    counter

    <button @click="handleAdd">Add</button>
  </div>
</template>