<script setup>
defineProps({
  title: {
    required: true,
    type: String,
  },
});
</script>

<template>
  <p class="title">{{ title }}</p>
</template>

<style scoped>
.title {
  font-size: 20px;
  line-height: 1.6;
  border: 1px solid rgba(var(--accent), 25%);
  background-color: white;
  padding: 1rem;
  border-radius: 0.4rem;
  color: rgb(var(--accent));
}
</style>
