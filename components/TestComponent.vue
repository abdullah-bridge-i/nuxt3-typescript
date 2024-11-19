<script lang="ts" setup>
defineProps<{ message: string }>();

const count = ref<number>(0);

function increment() {
  count.value++; // Correct type
}


</script>

<template>
  <div>
    <p>{{ message }}</p>
    <button @click="increment">Increment: {{ count }}</button>
  </div>
</template>
