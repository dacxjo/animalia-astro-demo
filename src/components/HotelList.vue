<script setup>
import Hotel from "./Hotel.vue";
defineProps({
  hotels: {
    default: [],
    type: Array,
  },
});
</script>

<template>
  <ul class="hotel-list">
    <Hotel v-for="h in hotels" :title="h.title.rendered"></Hotel>
  </ul>
</template>

<style scoped>
.hotel-list {
  border: 1px solid rgb(var(--accent));
  border-radius: 10px;
  filter: drop-shadow(40px);
  padding: 0 15px;
}
</style>
