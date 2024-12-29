
<script setup>
// this components is import on App1.vue
const props =defineProps([
    'label','modelValue'
])



const emit = defineEmits(['update:modelValue'])
</script>

<template>

    <label>{{ label }}</label><br>
    <input type="text" :value="modelValue" @input="emit('update:modelValue', $event.target.value)"/>
 
</template>

<style scoped></style>
