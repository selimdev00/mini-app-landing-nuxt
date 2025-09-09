<template>
  <div class="container">
    <div class="text-center max-w-[1048px] mx-auto space-y-6">
      <h1 class="font-unbounded text-[36px] font-medium">
        MiniApp — как новый “сайт”, только в Telegram
      </h1>

      <p class="text-text-gray text-2xl">
        Это приложение внутри Telegram с иконкой на главном экране. В нём можно
        удобно разместить навигацию по каналу, курсам и модулям, принять оплату,
        выдать доступ к урокам и напомнить подписчику о встрече.
      </p>
    </div>

    <div class="relative">
      <div
        class="gradient-secondary max-w-[382px] rounded-[16px] p-6 space-y-5 absolute right-1/12 top-6"
      >
        <h2 class="font-unbounded text-xl">Повышает вовлечённость</h2>

        <div class="border border-[rgba(255,255,255,0.4)]"></div>

        <div class="flex items-center gap-4">
          <div class="shrink-0">
            <icon-telegram />
          </div>

          <p class="text-sm">
            Вся информация прямо в телеграм,  без сторонних ссылок. Подписчики
            легко находят контент и чаще взаимодействуют.
          </p>
        </div>
      </div>

      <img
        src="@/assets/images/landing-2.png"
        alt=""
        class="block mx-auto mt-12"
      />

      <div
        class="gradient-secondary max-w-[382px] rounded-[16px] p-6 space-y-5 absolute left-1/12 bottom-6"
      >
        <h2 class="font-unbounded text-xl">Без сложны настроек</h2>

        <div class="border border-[rgba(255,255,255,0.4)]"></div>

        <div class="flex items-center gap-4">
          <p class="text-sm">
            Пользователям больше не нужно скроллить посты в поисках нужной
            информации. Или уходить на другие сервисы.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
