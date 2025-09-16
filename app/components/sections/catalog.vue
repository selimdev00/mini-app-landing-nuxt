<script setup lang="ts">
// const activeNav = ref();
//
// onMounted(() => {
//   activeNav.value = 0;
// });
//
// const nav = [
//   {
//     title: "Навигация по каналу",
//     items: [
//       {
//         image: new URL(
//           "@/assets/images/projects/navigation/1.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/navigation/2.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/navigation/3.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/navigation/4.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/navigation/5.png",
//           import.meta.url,
//         ).href,
//       },
//     ],
//   },
//   {
//     title: "Онбординг",
//     items: [
//       {
//         image: new URL(
//           "@/assets/images/projects/onboarding/1.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/onboarding/2.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/onboarding/3.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/onboarding/4.png",
//           import.meta.url,
//         ).href,
//       },
//       {
//         image: new URL(
//           "@/assets/images/projects/onboarding/5.png",
//           import.meta.url,
//         ).href,
//       },
//     ],
//   },
//   {
//     title: "Магазин",
//     items: [
//       {
//         image: new URL("@/assets/images/projects/store/1.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/store/2.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/store/3.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/store/4.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/store/5.png", import.meta.url)
//           .href,
//       },
//     ],
//   },
//   {
//     title: "Настройки",
//   },
//   {
//     title: "Внутренние страницы",
//     items: [
//       {
//         image: new URL("@/assets/images/projects/inner/1.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/inner/2.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/inner/3.png", import.meta.url)
//           .href,
//       },
//       {
//         image: new URL("@/assets/images/projects/inner/4.png", import.meta.url)
//           .href,
//       },
//     ],
//   },
//   {
//     title: "Мероприятия",
//   },
// ];
//
// const activeItem = computed(() => nav[activeNav.value]);

const images = import.meta.glob(
  "@/assets/images/projects2/*.{png,jpg,jpeg,gif}",
  {
    eager: true,
    import: "default",
  },
);
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

    <!--    <div-->
    <!--      class="flex justify-center gap-4 flex-wrap max-w-[868px] mx-auto mt-12"-->
    <!--    >-->
    <!--      <button-->
    <!--        v-for="(item, index) in nav"-->
    <!--        :key="item.title"-->
    <!--        class="font-unbounded font-bold border border-[#333333] py-[10px] px-[18px] rounded-[63px] md:text-base text-sm"-->
    <!--        :class="{ 'gradient-primary': index === activeNav }"-->
    <!--        @click="activeNav = index"-->
    <!--      >-->
    <!--        {{ item.title }}-->
    <!--      </button>-->
    <!--    </div>-->

    <div class="mt-15">
      <ui-carousel class="relative w-full">
        <ui-carousel-content>
          <ui-carousel-item
            v-for="(image, index) in images"
            :key="index"
            class="basis-1/2 xs:basis-1/2 sm:basis-1/3 md:basis-1/4 lg:basis-1/5 flex items-center justify-center"
          >
            <img :src="image" alt="" />
          </ui-carousel-item>
        </ui-carousel-content>

        <ui-carousel-previous></ui-carousel-previous>
        <ui-carousel-next></ui-carousel-next>
      </ui-carousel>
    </div>
  </div>
</template>
