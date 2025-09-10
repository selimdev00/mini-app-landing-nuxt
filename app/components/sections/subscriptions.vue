<script setup lang="ts"></script>

<template>
  <div class="container mt-[200px]">
    <div class="text-center max-w-[1122px] mx-auto space-y-6">
      <h1 class="font-unbounded text-[32px] font-medium">
        Подписка с возможностью помощи в настройке, а еще и на связи 24/7
      </h1>
    </div>

    <div class="grid grid-cols-[4fr_8fr] gap-6 mt-15">
      <div class="bg-secondary p-10 rounded-[24px] space-y-6">
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

          <p class="text-sm max-w-[261px]">
            Создайте своё мини-приложение для Telegram используя все
            возможности.
          </p>
        </div>

        <div class="flex gap-[14px]">
          <icon-list class="shrink-0" />

          <p class="text-sm max-w-[261px]">
            Разблокируйте неограниченное  кол-во доступов и аналитику навигации.
          </p>
        </div>

        <div class="flex gap-[14px]">
          <icon-support class="shrink-0" />

          <p class="text-sm max-w-[261px]">
            Тех. поддержка и помощь на любом этапе.
          </p>
        </div>

        <ui-button>Попробовать 7 дней бесплатно</ui-button>
      </div>

      <div
        class="bg-secondary p-10 rounded-[24px] space-y-6 relative overflow-hidden bg-[url('@/assets/images/subscriptions-image.png')] bg-no-repeat bg-[right_bottom]"
      >
        <h4
          class="font-unbounded text-xl font-medium relative inline-flex items-center"
        >
          Максимальная выгода с годовой подпиской

          <icon-discount-20 class="absolute -right-18" />
        </h4>

        <div
          class="bg-third rounded-[16px] p-4 flex items-center gap-[12px] justify-self-start"
        >
          <icon-checked class="text-purple" />

          <p class="text-xl font-medium flex items-center gap-[12px]">
            48 000 руб. / Год
            <span class="text-[#808080] text-sm">(4000 руб./месяц)</span>
          </p>
        </div>

        <div class="border border-[#333333]"></div>

        <div class="flex">
          <div class="space-y-6">
            <div class="flex gap-[14px]">
              <icon-layout class="shrink-0" />

              <p class="text-sm max-w-[261px]">
                Создайте своё мини-приложение для Telegram используя все
                возможности.
              </p>
            </div>

            <div class="flex gap-[14px]">
              <icon-list class="shrink-0" />

              <p class="text-sm max-w-[261px]">
                Разблокируйте неограниченное кол-во доступов и аналитику
                навигации.
              </p>
            </div>

            <div class="flex gap-[14px]">
              <icon-support class="shrink-0" />

              <p class="text-sm max-w-[261px]">
                Тех. поддержка и помощь на любом этапе.
              </p>
            </div>
          </div>

          <div class="flex gap-[14px]">
            <icon-paint-outline class="shrink-0" />

            <p class="text-sm max-w-[261px]">
              Получите бонусом разработку дизайна вашей навигации.
            </p>
          </div>
        </div>

        <ui-button variant="purple"
          >Попробовать с выгодой 12 000 руб.</ui-button
        >
      </div>
    </div>
  </div>
</template>
