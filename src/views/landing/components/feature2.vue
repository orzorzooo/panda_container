<template>
  <div class="py-20">
    <div class="row orzFeatures">
      <img
        :src="featureImgs[currentIndex].url"
        alt=""
        class="absolute min-h-full md:max-h-full md:w-full z-0 transition object-cover"
      />
      <div
        class="col-6 col-md-3 z-10"
        v-for="(item, index) in featureImgs"
        @mouseover="fuck(index)"
      >
        <div
          class="block border border-white h-full hover:bg-gray-500/50 transition"
        >
          <div
            class="p-3 text-center transition-all"
            :class="currentIndex == index ? 'h-auto bg-white' : 'h-0'"
          >
            <div
              class="text-xl text-gray-700 font-black"
              v-if="currentIndex == index"
            >
              {{ item.title }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import feature_1 from "@/assets/images/feature_1.jpg";
import feature_2 from "@/assets/images/feature_2.jpg";
import feature_3 from "@/assets/images/feature_3.jpg";
import feature_4 from "@/assets/images/feature_4.jpg";
import { ref } from "vue";

const featureImgs = [
  { url: feature_1, title: "模組化" },
  { url: feature_2, title: "可擴展" },
  { url: feature_3, title: "易維護" },
  { url: feature_4, title: "低成本" },
];
const currentIndex = ref(0);

function fuck(index) {
  console.log("fuck", index);
  currentIndex.value = index;
}
</script>
<style scoped>
.orzFeatures {
  height: 600px;
  position: relative;
  z-index: 0;
}
</style>
