<script setup>
import CardWideWithPlantVue from '../atom/CardWideWithPlant.vue';
import SectionTitle from '../atom/SectionTitle.vue';
</script>
<template>
    <section class="relative top-32 xl:top-16 2xl:top-96  px-6 py-3 z-10 lg:px-14 lg:py-16 w-full">
        <SectionTitle>Our Trendy Plant</SectionTitle>
        <div class="mt-16 md:mt-32 space-y-10 md:space-y-28 xl:space-y-40">
            <CardWideWithPlantVue direction="left" image="/trendyPlant.png" title="For Small Decs Ai Plat"
                description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua"
                price="599" />
            <CardWideWithPlantVue direction="right" image="/trendyPlant2.png" title="For Fresh Decs Ai Plat"
                description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua"
                price="579" />
        </div>
    </section>
</template>