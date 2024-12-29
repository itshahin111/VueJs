<script setup>
// this components is import on App1.vue
const props =defineProps([
    'person'
])


</script>

<template>

    
    <label>Name</label><br>
    <input type="text" v-model="person.name"/><br>
    <label>Email</label><br>
    <input type="text" v-model="person.email"/>
 
</template>

<style scoped></style>
