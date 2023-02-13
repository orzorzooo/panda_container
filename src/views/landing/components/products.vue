<template>
  <div>
    <div class="py-5 px-5 md:py-36 md:px-20">
      <div class="row">
        <div
          class="col-12 col-md-4 mb-10 md:p-4"
          v-for="(item, index) in models"
          :key="index"
        >
          <q-card class="p-4">
            <div class="text-center">
              <q-icon :name="item.icon"></q-icon>
            </div>

            <div>
              <div class="text-center mb-10">
                <h2 class="text-xl font-bold">{{ item.title }}</h2>
                <q-img :src="item.img" class="my-10"> </q-img>
              </div>
              <q-separator />
              <q-list class="text-md text-gray-700">
                <q-item>
                  <p class="">{{ item.main }}</p>
                </q-item>
                <q-item>
                  <p>{{ item.inside }}</p>
                </q-item>
                <q-item>
                  <p>{{ item.bathroom }}</p>
                </q-item>
                <q-item>
                  <p>{{ item.hardware }}</p>
                </q-item>
                <q-item>
                  <p>{{ item.option }}</p>
                </q-item>
              </q-list>
            </div>
            <div class="text-center text-gray-600 my-10">
              <p>開放客戶定制需求（具體方案需探討）</p>
            </div>
          </q-card>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
const models = [
  {
    icon: "mdi-octagram",
    title: "基礎型 | 8坪",
    main: " 鋼結構框架，外飾飾面板（鋁制）、隔熱、 保溫（100mm聚氨保溫層）、外牆玻璃 （6+12A+6中空LOW-E玻璃）、入戶門（智能 門禁）腳撐。",
    inside:
      "天花（竹炭纖維板）、牆面（竹炭纖維板）、 地面（高級複合木地板）、室內燈效（ 3000K 暖黃光）室外燈效（4000K暖白光）、窗簾 （電動窗簾）、智控系統（燈光、窗簾語音控 制）、消防煙霧報警、插座面板（品牌開關面 板）",
    bathroom:
      "馬桶（品牌馬桶）、熱水器（60L儲水式熱 水器）、台盆（品牌）龍頭（品牌） ",
    hardware:
      "空調（掛壁式1.5P空調2台）、熱水器、浴 霸（暖風式三合一集成浴霸） ",
    option: "地暖（電地暖）、水管防凍、投影儀、樓梯",
    img: new URL("/src/assets/images/rc/feature-01.png", import.meta.url),
  },
  {
    icon: "mdi-hexagram",
    title: "標準型 | 12坪",
    main: " 钢鋼結構框架，外飾飾面板（鋁制）、隔熱、保溫（100mm聚氨保溫層）、外牆玻璃 （6+12A+6中空LOW-E玻璃）、入戶門（智能門禁）腳撐。",
    inside:
      "天花（竹炭纖維板）、牆面（竹炭纖維板）、 地面（高級複合木地板）、室內燈效（ 3000K 暖黃光）室外燈效（4000K暖白光）、窗簾 （電動窗簾）、智控系統（燈光、窗簾語音控 制）、消防煙霧報警、插座面板（品牌開關面 板）",
    bathroom:
      "馬桶（品牌馬桶）、熱水器（60L儲水式熱 水器）、台盆（品牌）龍頭（品牌） ",
    hardware:
      "空調（掛壁式1.5P空調2台）、熱水器、浴 霸（暖風式三合一集成浴霸） ",
    option: "地暖（電地暖）、水管防凍、投影儀、樓梯",
    img: new URL("/src/assets/images/rc/feature-01.png", import.meta.url),
  },
  {
    icon: "mdi-shield-star",
    title: "豪華型 | 24坪",
    main: " 鋼結構框架，外飾飾面板（鋁制）、隔熱、 保溫（100mm聚氨保溫層）、外牆玻璃 （6+12A+6中空LOW-E玻璃）、入戶門（智能 門禁）腳撐。",
    inside:
      "天花（竹炭纖維板）、牆面（竹炭纖維板）、 地面（高級複合木地板）、室內燈效（ 3000K 暖黃光）室外燈效（4000K暖白光）、窗簾 （電動窗簾）、智控系統（全屋集成控制系 統，含背景音樂）、消防煙霧報警、插座面板 （品牌開關開關面板），傢俱：床、床墊、沙發、茶几。",
    bathroom:
      "馬桶（品牌馬桶）、熱水器（60L儲水式熱 水器）、台盆（品牌）龍頭（品牌） ",
    hardware:
      "冰箱、空調（品牌風管式空調）、熱水器 （即熱式熱水器）、浴霸（暖風式三合一 集成浴霸）投影儀",
    option: "地暖（電地暖）、水管防凍、投影儀、樓梯",
    img: new URL("/src/assets/images/rc/feature-01.png", import.meta.url),
  },
];
</script>
