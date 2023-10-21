<template>
  <div class="testimonial-card">
    <img
      :src="testimonial.image"
      :alt="testimonial.name"
      class="testimonial-img"
    />
    <div class="avatar-info">
      <h2 class="avatar-review">{{ testimonial.review }}</h2>
      <span class="avatar-name">{{ testimonial.name }}</span>
      <span class="avatar-star">{{ testimonial.stars }}</span>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(["testimonial"]);
</script>

<style scoped>
.testimonial-card {
  display: flex;
  align-items: center;
  gap: 1rem;
  max-width: 340px;
}
.testimonial-img {
  width: 50px;
  height: 50px;
  object-fit: contain;
  border-radius: 10rem;
}
.avatar-info {
  display: flex;
  align-items: start;
  flex-direction: column;
  gap: 0.5rem;
  background-color: #143a6f9f;
  border-radius: 0.4rem;

  padding: 1rem;
}
.avatar-review {
  font-weight: 300;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
.avatar-name {
  font-weight: 600;
}
</style>
