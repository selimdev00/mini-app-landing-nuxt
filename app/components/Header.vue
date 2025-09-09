<script setup lang="ts">
const links = [
  {
    title: "Возможности",
  },
  {
    title: "Для кого",
  },
  {
    title: "Как работает",
  },
  {
    title: "Подписка",
  },
  {
    title: "Вопросы",
  },
  {
    title: "Поддержка",
  },
];
</script>

<template>
  <header>
    <ul>
      <li v-for="(item, index) in links" :key="item.title">
        {{ item.title }}
      </li>
    </ul>
  </header>
</template>
