<script setup lang="ts">
import catalogImage from "@/assets/images/catalog-image.png";

const activeNav = ref(0);

const nav = [
  {
    title: "Навигация по каналу",
    items: [
      {
        image: catalogImage,
      },
    ],
  },
  {
    title: "Онбординг",
  },
  {
    title: "Магазин",
  },
  {
    title: "Настройки",
  },
  {
    title: "Внутрение страницы",
  },
  {
    title: "Мероприятия",
  },
];
</script>

<template>
  <div class="container mt-[200px]">
    <div class="text-center max-w-[794px] mx-auto space-y-6">
      <h1 class="font-unbounded text-[36px] font-medium">
        Мы сделали навигацию по каналу проще и удобнее
      </h1>

      <p class="text-text-gray text-2xl">
        Настраивай оформление, управляй подпиской  и расширяй права доступа в
        пару кликов из админ панели.
      </p>
    </div>

    <div
      class="flex justify-center gap-4 flex-wrap max-w-[868px] mx-auto mt-12"
    >
      <button
        v-for="(item, index) in nav"
        :key="item.title"
        class="font-unbounded font-bold border border-[#333333] py-[10px] px-[18px] rounded-[63px]"
        :class="{ 'gradient-primary': index === activeNav }"
        @click="activeNav = index"
      >
        {{ item.title }}
      </button>
    </div>

    <div v-if="nav[activeNav]" class="flex justify-between mt-15">
      <div v-for="item in 5">
        <img :src="catalogImage" alt="" />
      </div>
    </div>
  </div>
</template>
