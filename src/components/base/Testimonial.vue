<template>
  <section class="container">
    <div class="wrapper-testimonial mt px">
      <TestimonialCard
        v-for="testimonial in testimonials"
        :key="testimonial.name"
        :testimonial="testimonial"
      />
    </div>
  </section>
</template>
<style scoped>
.wrapper-testimonial {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  gap: 1rem;
}
</style>
<script setup>
import TestimonialCard from "../common/TestimonialCard.vue";

const testimonials = [
  {
    review: "Amazing product! Changed my life completely.",
    stars: "⭐⭐⭐⭐⭐",
    name: "Alice Johnson",
    image: "https://placekitten.com/100/100", // Placeholder image URL
  },
  {
    review: "Excellent service! Quick and efficient.",
    stars: "⭐⭐⭐⭐⭐",
    name: "Bob Smith",
    image: "https://placekitten.com/100/100", // Placeholder image URL
  },
  {
    review: "Couldn't be happier with my purchase. Top-notch quality!",
    stars: "⭐⭐⭐⭐⭐",
    name: "Charlie Davis",
    image: "https://placekitten.com/102/102", // Placeholder image URL
  },
  {
    review: "Outstanding customer support. Resolved my issue in no time.",
    stars: "⭐⭐⭐⭐⭐",
    name: "David Miller",
    image: "https://placekitten.com/103/103", // Placeholder image URL
  },
  {
    review: "Great value for money. Highly recommended!",
    stars: "⭐⭐⭐⭐⭐",
    name: "Eva Wilson",
    image: "https://placekitten.com/104/104", // Placeholder image URL
  },
  {
    review: "Impressive product design. Sleek and stylish!",
    stars: "⭐⭐⭐⭐⭐",
    name: "Frank Carter",
    image: "https://placekitten.com/105/105", // Placeholder image URL
  },
];
</script>
