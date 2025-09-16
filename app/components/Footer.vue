<template>
  <footer>
    <div class="container border-t mt-[100px] pt-10 pb-20">
      <div class="grid lg:grid-cols-[2fr_1fr] lg:gap-[224px] gap-4 text-lg">
        <div class="text-text-gray space-y-4 lg:order-1 order-2">
          <Logo class="lg:block hidden" />

          <p>© 2024. Все права защищены</p>

          <p>
            Индивидуальный предприниматель Новиков Алексей Сергеевич ИНН
            645120400330 ОГРНИП 325645700060363
          </p>

          <p>
            Используем cookies для корректной работы сайта, персонализации
            пользователей и других целей предусмотренных
            <nuxt-link to="#" class="text-white underline"
              >политикой конфеденциальности.
            </nuxt-link>
          </p>
        </div>

        <div class="lg:space-y-10 space-y-4 lg:order-2 order-1">
          <Logo class="lg:hidden block" />

          <h4 class="text-text-gray">Контакты</h4>

          <ul class="space-y-4">
            <li>
              <a class="flex gap-[12px]" href="tel:8 (800) 200-17-22">
                <icon-phone />8 (800) 200-17-22
              </a>
            </li>

            <li>
              <a class="flex gap-[12px]" href="mailto:info@marsakod.app">
                <icon-mail />

                info@marsakod.app</a
              >
            </li>
          </ul>

          <div class="flex gap-[12px]">
            <ui-button
              variant="secondary"
              as="a"
              href="https://t.me/marsakod_bot/app?startapp=ref-landingcap"
              target="_blank"
            >
              <icon-telegram class="text-[25px]" />
              <span class="lg:block hidden">Подпишитесь на нас в телеграм</span>
            </ui-button>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script setup lang="ts"></script>
