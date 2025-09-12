<template>
  <footer>
    <div class="container border-t mt-[100px] pt-10 pb-20">
      <div class="grid lg:grid-cols-[2fr_1fr] lg:gap-[224px] gap-4 text-lg">
        <div class="text-text-gray space-y-4 lg:order-1 order-2">
          <Logo />

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

        <div class="space-y-10 lg:order-2 order-1">
          <h4 class="text-text-gray">Контакты</h4>

          <ul class="space-y-4">
            <li class="flex gap-[12px]"><icon-phone />8 (800) 200-17-22</li>

            <li class="flex gap-[12px]"><icon-mail /> info@marsakod.app</li>
          </ul>

          <div class="flex gap-[12px]">
            <ui-button variant="secondary">
              <icon-telegram />
              <span class="lg:block hidden">Подпишитесь на нас в телеграм</span>
            </ui-button>

            <ui-button variant="secondary">
              <icon-vk class="text-2xl" />
            </ui-button>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
