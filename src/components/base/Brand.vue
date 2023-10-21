<template>
  <section class="container">
    <div class="brand-wrapper mt px">
      <p>Trusted by 30,000+ content, SEO, and marketing teams including…</p>
      <img src="@/assets/brand-img.png" alt="brand" class="brand-img" />
    </div>
  </section>
</template>

<style scoped>
.brand-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  row-gap: 2rem;
}
p {
  font-size: 1rem;
  font-weight: 500;
}
.brand-img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
</style>
