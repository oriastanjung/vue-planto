<script setup>
import Button from "../ui/Button.vue"
import CardWithPlant from "../atom/CardWithPlant.vue"
import CardFeedback from "../atom/CardFeedback.vue"
</script>

<template>
    <section class="relative top-24 2xl:top-72 px-6 py-3 z-10 lg:px-14 lg:py-16 w-full flex lg:flex-row flex-col justify-between items-center">
        <div class="flex flex-col lg:mr-20">
            <h2 class="font-extrabold text-5xl lg:text-8xl">Breath Natureal </h2>
            <p class="mt-3 font-light text-lg lg:text-2xl lg:w-11/12 2xl:w-7/12">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            <div class="flex mt-9">
                <Button>Explore</Button>
            </div>
            <div class="block mt-10 lg:mt-24 2xl:mt-48">
                <CardFeedback />
            </div>
        </div>
        <div class="flex mt-32 lg:mt-">
            <CardWithPlant image="/plant-hero.png" title="Calathea plant" category="Trendy House Plant" />
        </div>
    </section>
</template>