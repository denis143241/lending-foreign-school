<template>
  <div id="answer" class="answer-block">
    <div class="container">
      <div class="row">
        <div class="col m4 s12 wow fadeInLeft">
          <div class="answer-title">Ответы на популярные вопросы</div>
          <p class="subscription">
            Не нашли ответа на интересующий вопрос? Напишите нам в соцсетях или
            позвоните по номеру
          </p>
          <social-media />
          <h3>8 (904) 651-88-71</h3>
        </div>
        <div class="offset-m1 col m7 s12">
          <ul class="collapsible">
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Что такое пробный урок?
              </div>
              <div class="collapsible-body">
                <p>
                  Пробный урок абсолютно бесплатный. С помощью него вы получите
                  возможность опробовать нашу платформу обучения, пообщаься с
                  преподователем и уже после этого принять дальнейшее решение.
                </p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Пробный урок можно
                получить только после оплаты?
              </div>
              <div class="collapsible-body">
                <p>
                  Нет, пробный урок абсолютно бесплатный, его вы можете получить
                  в любой момент.
                </p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Что необходимо для
                обучения?
              </div>
              <div class="collapsible-body">
                <p>
                  Для обучения вам понадобится устройство с выходом в интернет,
                  микрофон и вебкамера.
                </p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Что если не получится
                прийти на урок?
              </div>
              <div class="collapsible-body">
                <p>
                  Ничего страшного, со всеми бывает. Обговорим перенос занятия и
                  назначим вам другое время.
                </p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Сколько времени
                придется уделять учебе?
              </div>
              <div class="collapsible-body">
                <p>
                  Для каждого человека мы стараемся подобрать личную программу
                  обучения. Все будет зависеть от того на сколько вам это нужно
                  :)
                </p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Сколько длится один
                урок?
              </div>
              <div class="collapsible-body">
                <p>Каждый урок длится 45 минут.</p>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-delay="30ms">
              <div class="collapsible-header">
                <span class="material-icons"> add </span>Когда происходит оплата
                за обучение?
              </div>
              <div class="collapsible-body">
                <p>Оплата за обучение происходит ежемесячно.</p>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import socialMedia from "./socialMedia.vue";
export default {
  components: {
    socialMedia,
  },
};
</script>

<style lang="less" scoped>
@import url("../assets/mainStyle.less");
.collapsible {
  box-shadow: none;
  border: none;
  &-header {
    font-weight: 500;
    padding: 20px 0;
  }
}
.material-icons {
  margin-right: 10px;
}
.answer {
  &-title {
    margin-top: 20px;
    font-family: @main-font;
    text-transform: uppercase;
    font-size: 38px;
    font-weight: 300;
    line-height: 130%;
    letter-spacing: normal;
    color: #000;
  }
  &-block {
    margin: 130px 0;
    font-family: @dop-font;
    font-size: 18px;
    letter-spacing: 0.9px;
    overflow: hidden;
  }
}
.subscription {
  font-weight: 900;
  font-size: 17px;
  margin: 40px 0;
}
h3 {
  font-size: 30px;
}
</style>

<style lang="less">
@import url("../assets/mainStyle.less");
.collapsible-body {
  border-bottom: 1px solid #f17f77 !important;
  border-top: 1px solid #f17f77 !important;
  color: @dop-color;
  font-size: 18px;
}
</style>
