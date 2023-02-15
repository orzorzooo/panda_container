<template>
  <div class="w-3/4 mx-auto">
    <q-toolbar class="q-gutter-x-md">
      <div class="font-bold text-xl">輕鋼構系列</div>
      <q-space></q-space>
      <div class="text-md text-gray-500" @click="$router.push({ name: 'lgs' })">
        關於輕鋼構
      </div>
    </q-toolbar>
    <q-separator />
  </div>
  <div class="w-3/4 mx-auto py-12">
    <h1 class="text-3xl font-bold text-center mb-12">選擇方案</h1>

    <div class="text-center">
      <q-btn-group flat>
        <q-btn
          v-for="item in datas"
          rounded
          outline
          :label="item.name"
          :color="currentSize == item.size ? 'primary' : 'grey-5'"
          size="xl"
          class="px-12 font-normal"
          @click="currentSize = item.size"
        />
      </q-btn-group>
    </div>
    <q-tab-panels
      v-model="currentSize"
      animated
      transition-prev="fade"
      transition-next="fade"
    >
      <q-tab-panel v-for="item in datas" :key="item.name" :name="item.size">
        <listItem :data="item.specs"></listItem>
      </q-tab-panel>
    </q-tab-panels>
    <div></div>
  </div>
</template>
<script setup>
import { ref } from "vue";
import listItem from "./components/listItem.vue";
import datas from "./components/datas";
const currentSize = ref("6");
</script>
