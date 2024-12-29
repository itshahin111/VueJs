<script setup>
import {ref, reactive } from 'vue'
import TextComponent from './components/TextComponent.vue'

const name = ref('Vue 3')
</script>

<template>

  <div>Orginal:{{ name }}</div>
  <h1>Text Component</h1>
  <div class="task-list">
    <label>
      <input type="text" v-model="name" />
    </label>
  </div>

  <div>
    <label>Text Component</label>
    <TextComponent v-model="name" />
  </div>
</template>

<style scoped>


</style>
