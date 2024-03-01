<script setup >
import TheWelcome from '../components/TheWelcome.vue'
import Navbar from "../components/layout/Navbar.vue"
import Hero from "../components/organism/Hero.vue"
</script>

<template>
  <Navbar />
  <main class="bg-[#1B2316] text-white w-full relative top-0 min-h-screen" >
    <div class="relative top-0"><img class="absolute top-0 z-0 h-2xl 2xl:w-full" src="/background.png" alt=""></div>
    <Hero />
  </main>
</template>
