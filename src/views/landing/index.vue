<template>
  <div class="h-800">
    <div class="relative">
      <img :src="c1" alt="" class="object-cover h-full" />
      <div class="absolute top-0 left-0 w-full h-full">
        <div class="flex justify-center items-center h-full">
          <div class="text-3xl font-bold text-white">Cool Container</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
import c1 from "@/assets/images/c-1.jpg";
</script>
