<script setup lang="ts"></script>

<template>
  <div
    class="bg-[url(@/assets/images/landing-bg.png)] bg-contain bg-right bg-no-repeat"
  >
    <div class="container">
      <div class="flex items-center h-screen">
        <div class="flex flex-col gap-6 items-start max-w-[780px]">
          <h1 class="font-unbounded text-[54px]">
            Навигация для твоего Телеграм-канала
          </h1>

          <p class="text-text-gray text-2xl">
            Конструктор навигации без затрат на разработку. Собери своё
            приложение с удобным доступом к материалам канала.
          </p>

          <ui-button>
            <svg
              width="25"
              height="20"
              viewBox="0 0 25 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M1.71862 8.60987C8.42949 5.78741 12.9045 3.92667 15.1435 3.02765C21.5365 0.460774 22.8649 0.0148807 23.7307 0.000156987C23.9212 -0.00308132 24.347 0.0424773 24.6228 0.25852C24.8557 0.440943 24.9197 0.687369 24.9504 0.860326C24.9811 1.03328 25.0192 1.42728 24.9889 1.73514C24.6424 5.249 23.1434 13.7762 22.3808 17.7118C22.0581 19.3771 21.4227 19.9354 20.8076 19.9901C19.4707 20.1088 18.4556 19.1372 17.1608 18.3179C15.1348 17.0358 13.9901 16.2377 12.0235 14.9867C9.75066 13.5408 11.224 12.7462 12.5193 11.4475C12.8583 11.1076 18.7484 5.93584 18.8624 5.46668C18.8767 5.40801 18.8899 5.18929 18.7553 5.0738C18.6207 4.95831 18.422 4.9978 18.2787 5.02921C18.0754 5.07373 14.8388 7.1389 8.56858 11.2247C7.64986 11.8337 6.8177 12.1304 6.07212 12.1149C5.25018 12.0977 3.6691 11.6663 2.49372 11.2974C1.05207 10.8451 -0.0937162 10.6059 0.00605648 9.83761C0.0580243 9.43745 0.628878 9.0282 1.71862 8.60987Z"
                fill="white"
              />
            </svg>

            Открыть в Телеграм
          </ui-button>
        </div>

        <div class="absolute right-0 max-w-[660px]">
          <img src="@/assets/images/landing.png" alt="" />
        </div>
      </div>
    </div>
  </div>

  <div class="container">
    <div class="text-center max-w-[1048px] mx-auto space-y-6">
      <h1 class="font-unbounded text-[54px]">
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
        class="gradient-primary max-w-[382px] rounded-[16px] p-6 space-y-5 absolute right-1/12 top-6"
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
        class="gradient-primary max-w-[382px] rounded-[16px] p-6 space-y-5 absolute left-1/12 bottom-6"
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
