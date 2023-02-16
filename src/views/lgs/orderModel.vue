<template>
  <div class="w-3/4 mx-auto mb-12">
    <q-toolbar class="q-gutter-x-md">
      <div class="font-bold text-xl">輕鋼構系列</div>
      <q-space></q-space>
      <div class="text-md text-gray-500" @click="$router.push({ name: 'lgs' })">
        關於輕鋼構
      </div>
    </q-toolbar>
    <q-separator />
  </div>
  <div class="w-3/4 mx-auto">
    <div class="row">
      <div class="col-5 pr-6">
        <img :src="img($route.params.size)" alt="" />
      </div>
      <div class="col pl-6">
        <div class="text-3xl font-bold">預約您的方案內容</div>
        <div class="text-3xl font-bold">
          {{ $route.params.size }}坪空間 | {{ $route.params.model }}配置
        </div>
        <q-separator class="my-6"></q-separator>
        <div class="mb-12 cursor-pointer">
          <div class="font-bold">選擇預約日期</div>
          <div
            class="font-bold text-lg p-6 border border-2 border-gray-300 rounded-xl"
          >
            <div>預約日期: {{ date }}</div>
            <q-popup-proxy
              cover
              transition-show="scale"
              transition-hide="scale"
            >
              <q-date v-model="date">
                <div class="row items-center justify-end">
                  <q-btn v-close-popup label="Close" color="primary" flat />
                </div>
              </q-date>
            </q-popup-proxy>
          </div>
        </div>
        <div>
          <div class="font-bold">客製化項目</div>
          <div
            class="font-bold text-lg p-6 border border-2 border-gray-300 rounded-xl mb-3"
          >
            水電
          </div>
          <div
            class="font-bold text-lg p-6 border border-2 border-gray-300 rounded-xl mb-3"
          >
            沙發、床具
          </div>
        </div>
      </div>
    </div>
  </div>
  <div
    class="fixed bottom-0 left-0 right-0 h-32 border-t border-gray-300 bg-gray-100"
  >
    <div class="row w-3/4 mx-auto py-6">
      <q-space></q-space>
      <div class="mr-6">
        <div class="text-2xl font-bold">NT$500,000</div>
        <div>預約後，我們將有專人與您聯繫</div>
      </div>
      <div>
        <q-btn size="md" color="primary">立即預約</q-btn>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
const img = (size) =>
  new URL(`/src/assets/images/lgs/size${size}.png`, import.meta.url);
const now = new Date();
const date = ref(now);
</script>
