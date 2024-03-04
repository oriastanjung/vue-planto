<script setup>

import TopSelling from "@/components/organism/TopSelling.vue";
import Navbar from "../components/layout/Navbar.vue"
import Hero from "../components/organism/Hero.vue"
import Trendy from "../components/organism/Trendy.vue"
import Footer from "../components/layout/Footer.vue"
</script>

<template>
  <Navbar />
  <main class="bg-[#1B2316] text-white w-full relative top-0 min-h-[330vh] md:min-h-[400vh] xl:min-h-[330vh] 2xl:min-h-[480vh]">
    <div class="relative top-0"><img class="absolute top-0 z-0 h-2xl 2xl:w-full" src="/background.png" alt=""></div>
    <Hero />
    <Trendy />
    <TopSelling />
  </main>
  <Footer />
</template>
