<template>
  <div>
    <div class="row">
      <div class="col h-96 md:h-screen">
        <orzImg :src="featureImg01">
          <div class="row text-gray-500">
            <div class="col-6 py-5 px-5 md:py-36 md:px-20">
              <div>
                <h2 class="text-6xl md:text-6xl font-thin mb-2 md:mb-5">
                  Light Gauge Steel Framing
                </h2>
                <h2 class="text-xl lg:text-8xl font-thin mb-2 md:mb-5">
                  輕鋼構系列
                </h2>
                <p class="md:text-md lg:text-lg font-bold">
                  抗震 | 抗風 | 防火 | 永續 | 舒適 | 快速 | 節能
                </p>
              </div>
              <q-btn
                color="primary"
                size="lg"
                @click="router.push({ name: 'lgs' })"
                >了解更多</q-btn
              >
            </div>
            <div class="col"></div>
          </div>
        </orzImg>
      </div>
    </div>
  </div>
</template>
<script setup>
import featureImg01 from "@/assets/images/lgs/feature-02.jpg";
import orzImg from "@/components/orzImg.vue";
import { useRouter } from "vue-router";
const router = useRouter();
</script>
