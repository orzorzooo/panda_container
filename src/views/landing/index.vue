<template>
  <!-- <div class="h-screen">
    <orzImg :src="c1">
      <div class="flex justify-center items-center h-full">
        <div class="text-3xl font-bold text-white">Cool Container</div>
      </div>
    </orzImg>
  </div> -->
  <hero></hero>
  <lgs></lgs>
  <container></container>
</template>
<script setup>
import { ref } from "vue";
import hero from "./components/hero.vue";
import feature from "./components/feature.vue";
import container from "./components/container.vue";
import orzImg from "@/components/orzImg.vue";
import lgs from "./components/lgs.vue";
</script>
