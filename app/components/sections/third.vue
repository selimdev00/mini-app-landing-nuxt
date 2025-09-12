<script setup lang="ts">
import { defineAsyncComponent } from "vue";

const sections = [
  {
    title: "Ваш проект будет уникальным",
    text: "Пользователям больше не нужно скроллить посты в поисках нужной информации. Или уходить на другие сервисы.",
    icon: defineAsyncComponent(() => import("@/components/icon/paint.vue")),
  },
  {
    title: "100% трафика в базе",
    text: "Вместо потерь вы получаете удержание и доходимость. Клуб живёт, дышит, растёт — и это видно по цифрам.",
    icon: defineAsyncComponent(() => import("@/components/icon/click.vue")),
  },
  {
    title: "Аналитика аудитории",
    text: "Вы получаете аналитику по активности, вовлечённости и мероприятиям. Знаете, кто активен, кто дремлет и почему.",
    icon: defineAsyncComponent(() => import("@/components/icon/analytics.vue")),
  },
  {
    title: "Одна навигация вместо 10 разных сервисов",
    text: "Сайт и магазин, чат-бот и рассылка, клуб по подписке, обучение, статистика канала, календарь и встречи, поиск единомышленников по городам и интересам.",
    icon: defineAsyncComponent(() => import("@/components/icon/catalog.vue")),
  },
  {
    title: "Новички не теряются",
    text: "Знакомьте пользователей с вашим каналам ещё до вступления.  Персональный онбординг для каждого участника, анкета с вопросами. ",
    icon: defineAsyncComponent(() => import("@/components/icon/user.vue")),
  },
  {
    title: "Сервис постоянно улучшается",
    text: "Постоянные обновления и бесплатный доступ к новому функционалу. Возможность разработать нужные вам модули приложения.",
    icon: defineAsyncComponent(() => import("@/components/icon/update.vue")),
  },
];
</script>

<template>
  <div id="possibilites" class="container pt-[100px]">
    <div class="text-center max-w-[787px] mx-auto md:space-y-6 space-y-4">
      <h1 class="font-unbounded md:text-[36px] text-lg font-medium">
        Зачем вам навигация внутри канала?
      </h1>

      <p class="text-text-gray md:text-2xl text-sm">
        Раньше такое могли позволить себе только крупные компании.  Мы сделали
        это доступным.
      </p>
    </div>

    <div
      class="grid xl:grid-cols-3 lg:grid-cols-2 gap-[14px] md:mt-[60px] mt-5"
    >
      <div
        v-for="(item, index) in sections"
        :key="item.title"
        class="min-h-[266px] bg-secondary rounded-[16px] p-6 space-y-5"
      >
        <div
          class="bg-third w-[60px] h-[60px] rounded-[12px] p-4 flex items-center justify-center"
        >
          <component :is="item.icon" />
        </div>

        <h3 class="font-unbounded text-xl font-medium">{{ item.title }}</h3>

        <div class="border border-third"></div>

        <p>{{ item.text }}</p>
      </div>
    </div>
  </div>
</template>
