<template>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Bungee+Spice&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap"
    rel="stylesheet"
  />
  <Header></Header>
  <main>
    <ComplianceGuide />
    <Slideshow />
    <FAQ />
    <IndustryExperts />
  </main>
  <Footer></Footer>
</template>

<script setup>
import ComplianceGuide from "./components/Compliance-guide.vue";
import FAQ from "./components/FAQ.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import IndustryExperts from "./components/Industry-experts.vue";
import Slideshow from "./components/Slideshow.vue";
</script>

<style scoped></style>
