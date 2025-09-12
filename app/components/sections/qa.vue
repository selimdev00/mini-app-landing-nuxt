<script setup lang="ts">
const questions = [
  {
    title: "Что такое MiniApp в Telegram?",
    content:
      "MiniApp — это встроенное приложение прямо внутри Telegram. Пользователь нажимает на кнопку и попадает в удобную навигацию, меню или витрину — как внутри полноценного сайта, но без переходов на внешние ссылки.",
  },
  {
    title: "Как собрать свой MiniApp?",
    content:
      "Вы можете собрать сами — у нас есть админка, гайды и видеоинструкции. Или заказать «под ключ» — мы соберём по вашему ТЗ, если нет ТЗ, ничего страшного, продумаем всю логику и заложим нужные бизнес-сценарии.",
  },
  {
    title: "Вы помогаете с дизайном?",
    content:
      "Да! У нас есть дизайнеры, которые делают стильные макеты для MiniApp. Хотите — используете свои. Хотите — заказываете у нас.",
  },
  {
    title: "Что делать, если мне нужен функционал, которого пока нет?",
    content:
      'Всегда можно обратиться к нам за любым не стандартным решением или интеграцией. По мимо реализации какого-то запроса под вас, вы можете оставить просто пожелания по улучшению, которые встают в очередь на бесплатную реализацию. У нас есть много функционала "под капотом", который не доступен пользователям в конструкторе, но который мы можем точечно подключать пользователям, если на него будет соответствующий запрос.',
  },
  {
    title: "Можно ли продавать MiniApp клиентам и зарабатывать?",
    content:
      "Да. У нас работает партнёрская программа. Вы находите клиентов — мы платим процент с оплаты.",
  },
  {
    title:
      "Есть ли ограничения по количеству разделов или материалов или количеству активных пользователей?",
    content:
      "Нет, ограничений никаких нет. Вы можете строить любую логику и глубину своего приложения.",
  },
  {
    title: "А если перестану платить — что будет?",
    content:
      "MiniApp перестанет быть доступен пользователям, но структура и данные останутся в вашем аккаунте. После завершения подписки, дается 3 дня для продления, до полного отключения. И 3 месяца до полного удаления. Можно оставить запрос в тех. поддержку, чтобы преднамеренно заморозили проект на длительный срок.",
  },
];
</script>

<template>
  <div
    id="qa"
    class="container flex lg:flex-nowrap flex-wrap pt-[100px] lg:gap-[125px] gap-5"
  >
    <div class="space-y-10 lg:min-w-[421px] w-full lg:order-1 order-2">
      <h3 class="font-unbounded text-[32px] font-medium lg:block hidden">
        Остались вопросы? Отвечаем
      </h3>

      <div
        class="bg-secondary p-10 rounded-[24px] space-y-4 bg-[url('@/assets/images/telegram.png')] bg-no-repeat bg-[right_top]"
      >
        <div class="space-y-[12px]">
          <icon-telegram class="text-purple text-[64px]" />

          <h4 class="font-unbounded text-xl font-medium">Поддержка</h4>
        </div>

        <div class="border border-[#333333]"></div>

        <div class="space-y-[12px]">
          <p>Чтобы задать вопрос, переходите в наш Телеграм.</p>

          <p>
            Мы ответим на любые вопросы и поможем с настройкой и разработкой
            Mini App
          </p>
        </div>

        <a
          href="https://t.me/marsakod_bot/app?startapp=ref-landinghelp"
          target="_blank"
        >
          <ui-button>Написать нам в телеграм</ui-button>
        </a>
      </div>
    </div>

    <div class="w-full lg:order-2 order-1">
      <h3
        class="font-unbounded text-[32px] font-medium lg:hidden block text-center"
      >
        Остались вопросы? Отвечаем
      </h3>

      <ui-accordion type="single" collapsible>
        <ui-accordion-item
          v-for="(item, index) in questions"
          :key="`question-${index}`"
          :value="`question-${index}`"
        >
          <ui-accordion-trigger>{{ item.title }}</ui-accordion-trigger>

          <ui-accordion-content>{{ item.content }}</ui-accordion-content>
        </ui-accordion-item>
      </ui-accordion>
    </div>
  </div>
</template>
