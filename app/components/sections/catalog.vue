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
  <div id="how-works" class="container pt-[100px]">
    <div class="text-center max-w-[794px] mx-auto space-y-6">
      <h1 class="font-unbounded md:text-[36px] text-lg font-medium">
        Мы сделали навигацию по каналу проще и удобнее
      </h1>

      <p class="text-text-gray md:text-2xl text-sm">
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
        class="font-unbounded font-bold border border-[#333333] py-[10px] px-[18px] rounded-[63px] md:text-base text-sm"
        :class="{ 'gradient-primary': index === activeNav }"
        @click="activeNav = index"
      >
        {{ item.title }}
      </button>
    </div>

    <div class="mt-15">
      <ui-carousel class="relative w-full">
        <ui-carousel-content>
          <ui-carousel-item
            v-for="item in 6"
            :key="item"
            class="basis-1/2 xs:basis-1/2 sm:basis-1/3 md:basis-1/4 lg:basis-1/5 flex items-center justify-center"
          >
            <img :src="catalogImage" alt="" />
          </ui-carousel-item>
        </ui-carousel-content>

        <ui-carousel-previous></ui-carousel-previous>
        <ui-carousel-next></ui-carousel-next>
      </ui-carousel>
    </div>
  </div>
</template>
