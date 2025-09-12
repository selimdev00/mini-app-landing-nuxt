<script setup lang="ts"></script>

<template>
  <div class="container mt-[100px]">
    <div class="text-center max-w-[1122px] mx-auto md:space-y-6 space-y-4">
      <h1 class="font-unbounded md:text-[32px] text-lg font-medium">
        Подписка с возможностью помощи в настройке, а еще и на связи 24/7
      </h1>
    </div>

    <div
      class="grid 2xl:grid-cols-[4fr_8fr] lg:grid-cols-2 gap-6 md:mt-15 mt-8"
    >
      <div class="bg-secondary md:p-10 p-5 rounded-[24px] space-y-6">
        <h4 class="font-unbounded text-xl font-medium">Ежемесячная подписка</h4>

        <div
          class="bg-third rounded-[16px] p-4 flex items-center gap-[12px] justify-self-start"
        >
          <icon-checked class="text-primary" />

          <p class="text-xl font-medium">5 000 руб. / Месяц</p>
        </div>

        <div class="border border-[#333333]"></div>

        <div class="flex gap-[14px]">
          <icon-layout class="shrink-0" />

          <p class="text-sm md:max-w-[261px]">
            Создайте своё мини-приложение для Telegram используя все
            возможности.
          </p>
        </div>

        <div class="flex gap-[14px]">
          <icon-list class="shrink-0" />

          <p class="text-sm md:max-w-[261px]">
            Разблокируйте неограниченное  кол-во доступов и аналитику навигации.
          </p>
        </div>

        <div class="flex gap-[14px]">
          <icon-support class="shrink-0" />

          <p class="text-sm md:max-w-[261px]">
            Тех. поддержка и помощь на любом этапе.
          </p>
        </div>

        <ui-button
          as="a"
          href="https://t.me/marsakod_bot/app?startapp=ref-landing7day"
          target="_blank"
          class="md:block hidden w-fit"
          >Попробовать 7 дней бесплатно</ui-button
        >
        <ui-button
          as="a"
          href="https://t.me/marsakod_bot/app?startapp=ref-landing7day"
          target="_blank"
          class="md:hidden block w-full text-center"
          >Попробовать бесплатно</ui-button
        >
      </div>

      <div
        class="bg-secondary md:p-10 p-5 rounded-[24px] space-y-6 relative overflow-hidden 2xl:bg-[url('@/assets/images/subscriptions-image.png')] bg-no-repeat bg-[right_bottom]"
      >
        <h4
          class="font-unbounded text-xl font-medium relative inline-flex items-center"
        >
          Максимальная выгода с годовой подпиской

          <icon-discount-20 class="2xl:block hidden absolute -right-18" />
        </h4>

        <div
          class="bg-third rounded-[16px] p-4 flex items-center gap-[12px] justify-self-start"
        >
          <icon-checked class="text-purple" />

          <p
            class="md:text-xl text-base font-medium flex flex-wrap items-center gap-x-[12px]"
          >
            48 000 руб. / Год
            <span class="text-[#808080] text-sm">(4000 руб./месяц)</span>
          </p>
        </div>

        <div class="border border-[#333333]"></div>

        <div class="flex gap-4 md:flex-nowrap flex-wrap">
          <div class="space-y-6">
            <div class="flex gap-[14px]">
              <icon-layout class="shrink-0" />

              <p class="text-sm md:max-w-[261px]">
                Создайте своё мини-приложение для Telegram используя все
                возможности.
              </p>
            </div>

            <div class="flex gap-[14px]">
              <icon-list class="shrink-0" />

              <p class="text-sm md:max-w-[261px]">
                Разблокируйте неограниченное кол-во доступов и аналитику
                навигации.
              </p>
            </div>

            <div class="flex gap-[14px]">
              <icon-support class="shrink-0" />

              <p class="text-sm md:max-w-[261px]">
                Тех. поддержка и помощь на любом этапе.
              </p>
            </div>
          </div>

          <div class="flex gap-[14px]">
            <icon-paint-outline class="shrink-0" />

            <p class="text-sm md:max-w-[261px]">
              Получите бонусом разработку дизайна вашей навигации.
            </p>
          </div>
        </div>

        <ui-button
          class="hidden md:block w-fit"
          variant="purple"
          as="a"
          href="https://t.me/marsakod_bot/app?startapp=ref-landing12m"
          target="_blank"
          >Попробовать с выгодой 12 000 руб.</ui-button
        >

        <ui-button
          class="block md:hidden w-full text-center"
          variant="purple"
          as="a"
          href="https://t.me/marsakod_bot/app?startapp=ref-landing12m"
          target="_blank"
          >Оформить</ui-button
        >
      </div>
    </div>
  </div>
</template>
