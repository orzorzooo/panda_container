<template>
  <div class="h-screen">
    <vueper-slides fixed-height="100vh">
      <vueper-slide
        v-for="(slide, i) in slides"
        :key="i"
        :title="slide.title"
        :content="slide.content"
        :image="slide.image"
      >
      </vueper-slide>
    </vueper-slides>
  </div>
</template>
<script setup>
import { ref } from "vue";
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
import c1 from "@/assets/images/c-1.jpg";
const slides = ref([
  {
    title: "",
    content: "",
    // You can also provide a URL for the image.
    image: c1,
  },
]);
</script>
