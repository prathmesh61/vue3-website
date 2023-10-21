<template>
  <section class="section">
    <div class="px container hero-wrapper mt">
      <h1 class="hero-heading">Smart AI for Smarter SEO</h1>
      <p class="hero-para">
        Frase is the fastest and easiest way to create content that ranks on
        Google.
      </p>
      <button class="btn">Get Start</button>
      <img src="@/assets/Hero.png" alt="Hero" class="main-Img" />
    </div>
    <img src="@/assets/haroBg.png" alt="Hero-Background" class="hero-bg" />
  </section>
</template>

<style scoped>
.section {
  position: relative;
}
.hero-bg {
  position: absolute;
  width: 100%;
  height: auto;
  object-fit: contain;
  top: 0%;
  opacity: 50%;
}
.hero-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 2rem;
}
.hero-heading {
  font-size: 4.1rem;
  font-weight: 700;
  text-align: center;
}
.hero-para {
  font-size: 1.1rem;
  text-align: center;
}
.main-Img {
  width: 80%;
  height: 80%;
  object-fit: cover;
  margin-top: 3rem;
}
</style>
