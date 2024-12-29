<script setup>
import { reactive } from 'vue'
import PersonComponent from './components/PersonComponent.vue'


const person = reactive({
  name: 'Vue 3',
  email: 'email@vue.com'
})

</script>


<template>
  
  <div class="">
    Original:{{ person.name }}<br/>
    Original :{{ person.email}}
    </div>
  <h1>Text Component</h1>
  <div class="task-list">
    <label>
      <input type="text" v-model="person.name" />
    </label>
  </div>

  <div>
    <label>Person Component</label>
    <PersonComponent :person="person" />
  </div>
</template>

<style scoped>


</style>
