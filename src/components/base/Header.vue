<template>
  <header class="container">
    <div class="wrapper">
      <img src="@/assets/logo.png" alt="logo" class="logo" />
      <div class="links-wrapper">
        <span class="link">Price</span>
        <span class="link">Resource</span>
        <span class="link">Login</span>
      </div>
      <button class="btn">Get Start</button>
    </div>
  </header>
</template>

<script setup></script>

<style scoped>
.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}
.logo {
  width: 250px;
  height: 35px;
  object-fit: contain;
}
.links-wrapper {
  display: flex;
  align-items: center;
  gap: 2rem;
}
.link {
  font-size: 1.1rem;
  font-weight: 400;
}
@media (max-width: 600px) {
  .links-wrapper {
    display: none;
  }
  .wrapper {
    justify-content: center;
  }
}
</style>
