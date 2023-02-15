<template>
  <div>
    <div class="w-1/2 mx-auto">
      <q-tabs
        v-model="tab"
        class="text-grey tab-text"
        content-class="!text-8xl"
        active-color="primary"
        indicator-color="primary"
        align="justify"
        narrow-indicator
      >
        <q-tab name="6" label="6坪" />
        <q-tab name="12" label="12坪" />
        <q-tab name="24" label="24坪" />
      </q-tabs>
    </div>
    <div class="w-2/3 mx-auto py-20">
      <q-tab-panels
        v-model="tab"
        animated
        transition-prev="fade"
        transition-next="fade"
      >
        <q-tab-panel name="6">
          <listItem :data="data6"></listItem>
        </q-tab-panel>

        <q-tab-panel name="12">
          <listItem :data="data12"></listItem>
        </q-tab-panel>
        <q-tab-panel name="24">
          <listItem :data="data24"></listItem>
        </q-tab-panel>
      </q-tab-panels>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
import listItem from "./listItem.vue";
import { data6, data12, data24 } from "./data";
const tab = ref("6");
</script>
<style scoped>
.orz-item {
  font-weight: 600;
}
</style>
