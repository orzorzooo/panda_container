<template>
  <div class="md:h-screen md:mb-24 py-20">
    <div class="w-1/2 relative z-1 text-3xl md:text-9xl font-black">
      <div class="text-gray-400">ELEGANCE</div>
      <div class="text-white">SPACES</div>
      <img :src="line01" alt="" class="absolute right-0 md:-top-8" />
    </div>

    <div class="relative md:-top-24">
      <!-- <img :src="line01" alt="" class="absolute w-1/2 right-0 top-0" /> -->
      <img :src="containerHeroBg" alt="" class="w-full" />
    </div>
    <!-- <vueper-slides fixed-height="100vh">
      <vueper-slide
        v-for="(slide, i) in slides"
        :key="i"
        :title="slide.title"
        :content="slide.content"
        :image="slide.image"
      >
      </vueper-slide>
    </vueper-slides> -->
  </div>
</template>
<script setup>
import { ref } from "vue";
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
import c1 from "@/assets/images/c-1.jpg";
import containerHeroBg from "@/assets/images/containerHero_bg.png";
import line01 from "@/assets/images/line01.svg";
const slides = ref([
  {
    title: "",
    content: "",
    // You can also provide a URL for the image.
    // image: con,
  },
]);
</script>
