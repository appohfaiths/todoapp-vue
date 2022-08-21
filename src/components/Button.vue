<script setup>
const props = defineProps({
  text: String,
});

function onClick() {
  console.log('clicked');
}
</script>

<template>
  <button
    @click="onClick()"
    class="inline-block bg-green-700 text-white px-4 py-2 m-1 rounded cursor-pointer text-base capitalize"
  >
    {{ text }}
  </button>
</template>
