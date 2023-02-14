<template>
  <div class="py-5 px-5 md:py-36 md:px-20 text-gray-500">
    <div class="row">
      <div class="col-12 col-md-6">
        <h1 class="text-6xl md:text-6xl font-thin">Container House</h1>
        <h2 class="text-xl lg:text-8xl font-thin mb-2 md:mb-5">組合系列</h2>
        <p class="text-xl">
          移動房屋，被廣泛應用於旅遊度假村、房車營地、創意園、商鋪等領域，為特色小鎮鋪設
          生態旅遊、移動地產、移動零售、打造旅居商一體的“移動商機”，自由組合可以靈活應用在不
          同的小鎮需求。
        </p>
        <q-btn color="primary" size="lg">了解更多</q-btn>
      </div>
      <div class="col-12 col-md-6">
        <div class="md:px-8 px-0">
          <img :src="featureImg" class="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import featureImg from "@/assets/images/rc/feature-01.png";
</script>
<style scoped>
.borderR {
  border-top-left-radius: 9999px;
  border-bottom-left-radius: 9999px;
}
</style>
