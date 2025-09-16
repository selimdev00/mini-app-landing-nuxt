<template>
  <div
    class="bg-[url(@/assets/images/landing-bg.png)] bg-contain bg-right bg-no-repeat"
  >
    <div
      class="flex items-center 2xl:h-screen 2xl:mt-0 md:mt-[200px] mt-[100px]"
    >
      <div class="container">
        <div
          class="flex flex-col md:gap-6 gap-4 2xl:items-start 2xl:items-center 2xl:max-w-[780px] relative z-10 2xl:mx-0 mx-auto"
        >
          <div
            class="py-2 px-[12px] rounded-[4px] text-primary bg-primary/20 md:mx-4 self-start"
          >
            Мini App в Телеграм
          </div>

          <h1
            class="font-unbounded md:text-[54px] text-[24px] font-medium md:px-4"
          >
            Навигация для твоего Телеграм-канала
          </h1>

          <p class="text-text-gray md:text-2xl text-sm md:px-4">
            Конструктор навигации без затрат на разработку. Собери своё
            приложение с удобным доступом к материалам канала.
          </p>

          <img
            src="@/assets/images/landing-mobile.png"
            alt=""
            class="max-w-[200%] w-[110%] relative right-4 2xl:hidden md:hidden block"
          />

          <div
            class="px-4 w-full flex md:justify-start justify-center md:mt-0 mt-5"
          >
            <a
              href="https://t.me/marsakod_bot/app?startapp=ref-landing"
              target="_blank"
            >
              <ui-button>
                <icon-telegram class="text-[25px]" />

                Открыть в Телеграм
              </ui-button>
            </a>
          </div>
        </div>
      </div>

      <div class="2xl:block hidden absolute right-0 max-w-[660px]">
        <img src="@/assets/images/landing.png" alt="" />
      </div>
    </div>
  </div>
</template>
