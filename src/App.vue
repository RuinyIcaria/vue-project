<script setup lang="ts">
import { ref } from 'vue'

const username = ref('123')
const password = ref('666')
</script>

<template>
  <div class="form">
    <span>{{ username }}</span>
    {{ password }}
  </div>
  <div class="form">

    <input placeholder="username" v-model="username" />
    <input placeholder="password" v-bind:value="password"/>
    <button @click="() => {username = '456'}">submit</button>
  </div>
</template>

<style>
.form>* {
  display: block;
}
</style>