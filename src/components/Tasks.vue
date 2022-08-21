<script setup>
const props = defineProps({
  tasks: Array,
});
</script>

<template>
  <div :key="task.id" v-for="task in tasks">
    <h3>{{ task.text }}</h3>
  </div>
</template>
