<template>
  <div class="container mt-[100px]">
    <div
      class="gradient-secondary rounded-[24px] sm:py-5 relative flex items-center"
    >
      <div class="max-w-[835px] lg:pl-10 lg:pt-9 md:p-9 p-8">
        <div class="space-y-6 lg:text-left text-center">
          <h1 class="font-unbounded md:text-[32px] text-lg font-medium">
            Разработка Mini App в вашем стиле от опытной команды специалистов
          </h1>

          <p class="text-text-gray md:text-xl text-sm">
            Любые индивидуальные решения и кастомизацией любой сложности, от
            интеграции с CRM и AI-инструментами, до любых желаемых модулей
            (рандом-кофе, тиндер, форум, и т.д.).
          </p>

          <a
            href="https://t.me/marsakod_bot/app?startapp=ref-landingdev"
            target="_blank"
            class="lg:hidden block w-full"
          >
            <ui-button class="w-full">
              <icon-telegram />
              Написать в телеграм
            </ui-button>
          </a>
        </div>

        <div
          class="lg:block hidden bg-background space-y-[12px] max-w-[438px] p-5 rounded-[16px] mt-9"
        >
          <h3 class="text-xl font-unbounded font-medium">
            Хотите свой Mini App?
          </h3>

          <div class="border border-[#363636]"></div>

          <p class="text-sm">
            Подключаем Яндекс.Метрику, CRM, платёжные системы  и другие сервисы
            для удобного управления и аналитики.
          </p>

          <p class="text-sm">
            Разработаем и продумаем приложение. Берём на себя все этапы — от
            идеи, проектирования до запуска и технической поддержки.
          </p>

          <a
            href="https://t.me/marsakod_bot/app?startapp=ref-landingdev"
            target="_blank"
            class="w-full"
          >
            <ui-button class="w-full"
              ><icon-telegram /> Написать в телеграм</ui-button
            >
          </a>
        </div>
      </div>

      <div class="lg:block hidden absolute right-0">
        <img src="@/assets/images/banner-image.png" alt="" />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts"></script>
