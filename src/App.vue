<script setup>
import { ref } from 'vue';
import Header from './components/Header.vue';
import Tasks from './components/Tasks.vue';

const tasks = ref([
  {
    id: 1,
    text: 'Doctors Appointment',
    day: 'March 1st at 2:30pm',
    reminder: true,
  },
  {
    id: 2,
    text: 'Meeting at School',
    day: 'March 3rd at 1:30pm',
    reminder: true,
  },
  {
    id: 3,
    text: 'Food Shopping',
    day: 'March 3rd at 11:00am',
    reminder: false,
  },
]);
</script>

<template>
  <div class="container mx-auto border border-slate-300 w-96 mt-4">
    <Header name="Melo" />
    <Tasks :tasks="tasks" />
  </div>
</template>

<style scoped></style>
