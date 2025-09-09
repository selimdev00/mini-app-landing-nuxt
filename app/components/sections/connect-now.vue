<script setup lang="ts">
const items = [
  {
    title: "Рост конверсий и автоматизация продаж",
  },
  {
    title: "Удобство для пользователей",
  },
  {
    title: "Больше вовлеченнось, меньше рутины",
  },
  {
    title: "Персонализация бренда",
  },
];
</script>

<template>
  <div class="container mt-[200px]">
    <div class="text-center max-w-[923px] mx-auto space-y-6">
      <h1 class="font-unbounded text-[36px] font-medium">
        Подключите Mini App сейчас  и получите преимущество в своей нише
      </h1>

      <p class="text-text-gray text-2xl">
        от блогеров и экспертов до онлайн школ и магазинов
      </p>
    </div>

    <div class="flex justify-center gap-[46px] items-center mt-[60px]">
      <div>
        <img src="@/assets/images/connect-now.png" alt="" />
      </div>

      <div class="space-y-4">
        <div
          v-for="item in items"
          :key="item.title"
          class="flex items-center bg-third p-4 rounded-[12px] gap-[12px]"
        >
          <icon-checked />

          <p class="text-xl font-medium">{{ item.title }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
