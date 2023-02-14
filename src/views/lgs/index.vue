<template>
  <div class="w-3/4 mx-auto">
    <q-toolbar class="q-gutter-x-md">
      <div class="font-bold text-xl">輕鋼構系列</div>
      <q-space></q-space>
      <div class="text-md text-gray-500">關於輕鋼構</div>
      <q-btn rounded size="sm" color="primary">訂購</q-btn>
    </q-toolbar>
    <q-separator />
  </div>
  <div>
    <img :src="img_01" alt="" class="w-full" />
  </div>
  <div class="py-20 text-gray-500 w-2/3 mx-auto text-center leading-loose">
    <h1 class="text-6xl font-bold mb-10">舒適</h1>
    <p class="text-3xl font-bold">
      牆壁、樓板、屋頂都是用複合多層式工法，防水毯、防火吸音隔熱材、外牆通氣構造等，達到防水、防火、隔音、吸震、冬暖夏涼之效果，由於沒有水泥牆體，也就沒有壁癌的問題產生。
    </p>
  </div>
  <div
    class="py-20 text-gray-500 w-2/3 mx-auto text-center leading-loose bg-gray-400"
  >
    <h1 class="text-6xl font-bold mb-10">舒適</h1>
    <p class="text-3xl font-bold">
      牆壁、樓板、屋頂都是用複合多層式工法，防水毯、防火吸音隔熱材、外牆通氣構造等，達到防水、防火、隔音、吸震、冬暖夏涼之效果，由於沒有水泥牆體，也就沒有壁癌的問題產生。
    </p>
  </div>
</template>
<script setup>
import img_01 from "@/assets/images/lgs/feature-03.jpg";
</script>
