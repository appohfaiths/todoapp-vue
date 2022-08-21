<script setup>
import Button from './Button.vue';
const props = defineProps({
  name: String,
});
</script>

<template>
  <header class="p-2 flex justify-between items-center">
    <h1>Task Tracker by {{ name }}</h1>
    <Button text="add task" />
  </header>
</template>
