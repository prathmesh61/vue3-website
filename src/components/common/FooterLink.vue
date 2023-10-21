<template>
  <span class="link">{{ item.name }}</span>
</template>

<script setup>
const props = defineProps(["item"]);
</script>

<style scoped>
.link {
  font-size: 1rem;
  cursor: pointer;
  font-family: Georgia, "Times New Roman", Times, serif;
}
</style>
