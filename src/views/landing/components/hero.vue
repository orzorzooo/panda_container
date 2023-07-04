<template>
  <div class="h-screen mb-24 py-20">
    <div class="text-9xl font-black text-gray-400">ELEGANCE</div>
    <div class="text-9xl font-black text-white">SPACES</div>
    <div class="relative -top-24">
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
const slides = ref([
  {
    title: "",
    content: "",
    // You can also provide a URL for the image.
    // image: con,
  },
]);
</script>
