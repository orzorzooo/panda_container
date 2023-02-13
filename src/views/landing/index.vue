<template>
  <div class="h-screen">
    <orzImg :src="c1">
      <div class="flex justify-center items-center h-full">
        <div class="text-3xl font-bold text-white">Cool Container</div>
      </div>
    </orzImg>
  </div>
  <lgs></lgs>
  <container></container>
  <products></products>
</template>
<script setup>
import { ref } from "vue";
import feature from "./components/feature.vue";
import container from "./components/container.vue";
import products from "./components/products.vue";
import orzImg from "@/components/orzImg.vue";
import lgs from "./components/lgs.vue";
import c1 from "@/assets/images/c-1.jpg";
</script>
