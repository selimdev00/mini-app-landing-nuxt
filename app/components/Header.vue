<script setup lang="ts">
import { useWindowScroll } from "@vueuse/core";

const links = [
  {
    title: "Возможности",
    href: "#",
  },
  {
    title: "Для кого",
    href: "#",
  },
  {
    title: "Как работает",
    href: "#",
  },
  {
    title: "Подписка",
    href: "#",
  },
  {
    title: "Вопросы",
    href: "#",
  },
  {
    title: "Поддержка",
    href: "#",
  },
];

const mobileMenu = ref(false);

const { y } = useWindowScroll();
</script>

<template>
  <header
    class="fixed top-0 w-full z-20 transition-colors"
    :class="{
      'bg-background': y > 100,
      'bg-transparent': y < 100,
    }"
  >
    <div class="container flex justify-between items-center py-6">
      <Logo />

      <div class="flex items-center gap-6">
        <ul class="xl:flex hidden gap-[22px]">
          <li v-for="(item, index) in links" :key="item.title">
            <nuxt-link :to="item.href" class="text-[18px]">{{
              item.title
            }}</nuxt-link>
          </li>
        </ul>

        <div class="flex gap-2">
          <ui-button
            class="xl:hidden block"
            variant="secondary"
            @click="mobileMenu = true"
          >
            <icon-hamburger class="text-xl" />
          </ui-button>

          <ui-button
            variant="secondary"
            as="a"
            href="https://t.me/marsakod_bot/app?startapp=ref-landingcap"
            target="_blank"
          >
            <icon-telegram class="text-xl" />

            <span class="hidden md:block">Открыть в Телеграм</span>
          </ui-button>
        </div>
      </div>
    </div>
  </header>

  <transition-slide>
    <div
      class="md:hidden block fixed top-0 right-0 w-full h-full bg-background max-w-[260px] z-20"
      v-if="mobileMenu"
    >
      <div class="p-4 flex flex-col gap-12 items-end">
        <div class="flex justify-end">
          <ui-button variant="secondary" @click="mobileMenu = false">
            <icon-x class="text-2xl" />
          </ui-button>
        </div>

        <Logo />

        <ul class="flex flex-col gap-[22px] text-right">
          <li v-for="(item, index) in links" :key="item.title">
            <nuxt-link :to="item.href" class="text-[18px]"
              >{{ item.title }}
            </nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </transition-slide>
</template>
