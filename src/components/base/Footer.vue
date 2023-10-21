<template>
  <footer class="bg-white">
    <section class="container footer-wrapper mt">
      <div class="footer-logo">
        <h2>Frase</h2>
        <p>Frase is transforming SEO and content creation with AI.</p>
      </div>
      <div class="footer-links">
        <FooterLink v-for="item in home" :item="item" :key="item.name" />
      </div>
      <div class="footer-links">
        <FooterLink v-for="item in resource" :item="item" :key="item.name" />
      </div>
      <div class="footer-links">
        <FooterLink v-for="item in company" :item="item" :key="item.name" />
      </div>
    </section>
  </footer>
</template>

<script setup>
import FooterLink from "../common/FooterLink.vue";
const home = [
  { name: "Home", link: "/home" },
  { name: "Services", link: "/services" },
  { name: "About Us", link: "/about-us" },
  { name: "Blog", link: "/blog" },
  { name: "Contact Us", link: "/contact" },
];
const resource = [
  { name: "SEO Packages", link: "/seo-packages" },
  { name: "Case Studies", link: "/case-studies" },
  { name: "Testimonials", link: "/testimonials" },
  { name: "FAQs", link: "/faqs" },
  { name: "Privacy Policy", link: "/privacy-policy" },
];
const company = [
  { name: "Client Portal", link: "/client-portal" },
  { name: "Free SEO Analysis", link: "/free-seo-analysis" },
  { name: "Careers", link: "/careers" },
  { name: "Terms of Service", link: "/terms-of-service" },
  { name: "Sitemap", link: "/sitemap" },
];
</script>

<style scoped>
.bg-white {
  background: #fff;
  color: #111;
}
.footer-logo {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
.footer-logo h2 {
  font-size: 1.5rem;
}
.footer-logo p {
  font-size: 1rem;
}
.footer-wrapper {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 2rem;
  padding: 2rem;
}
.footer-links {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
</style>
