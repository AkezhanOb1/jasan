<template>
  <header class="header">

    <div class="header__top">

      <div class="header__container header__container--top">

        <div class="header__logo-box" v-scroll-to="{el: '#welcome', duration: 700, offset: -140}">

          <img src="../assets/img/logo-jasan.png" alt="" class="header__logo">

          <div class="header__grey-text">
            Самые эффективные CRM <br>
            услуги в Казахстане
          </div>

        </div>

        <div class="header__socials">
          <a class="header__social">
            <svg width="25" height="25" @click="linker(`https://www.instagram.com/jasan_technologies/`)">
              <use href="../assets/img/icons.svg#header-inst"></use>
            </svg>
          </a>

          <a  class="header__social">
            <svg width="25" height="25" @click="linker(`https://www.facebook.com/jasankz/`)">
              <use href="../assets/img/icons.svg#header-fb"></use>
            </svg>
          </a>
        </div>

        <div class="header__call-box">
          <a href="tel: +7 (777) 205 93 39" class="header__phone-text">
            +7 (777) 2059339
          </a>
          <a class="header__call-order" v-scroll-to="{el: '#contact', duration: 700, offset: -160}">
            Заказать обратный звонок
          </a>
        </div>

        <div class="header__mail-box">

          <svg width="56" height="56">
            <use href="../assets/img/icons.svg#mail-box"></use>
          </svg>

          <div class="header__mail-info">
            <h6>
              Напишите нам
            </h6>
            <p>
              info@jasan.kz
            </p>
          </div>

        </div>

        <img src="../assets/img/icons/burger.svg" alt="" class="header__burger" @click="sidebarOpen = true">
      </div>

    </div>

    <div class="header__bottom">
      <div class="header__container header__container--bottom">
        <div class="header__item" v-scroll-to="{el: '#welcome', duration: 700, offset: -140}">Главная</div>
        <div class="header__item" v-scroll-to="{el: '#services', duration: 700, offset: -160}">Услуги</div>
        <div class="header__item" v-scroll-to="{el: '#bitrix', duration: 700, offset: -160}">Битрикс24</div>
        <div class="header__item" v-scroll-to="{el: '#steps', duration: 700, offset: -160}">Заявка</div>
        <div class="header__item" v-scroll-to="{el: '#contact', duration: 700, offset: -160}">Контакты</div>
      </div>
    </div>

    <div class="header__sidebar sidebar" :class="{'sidebar--active' : sidebarOpen}">

      <img src="../assets/img/icons/close.png" alt="" class="sidebar__close" @click="sidebarOpen = false">

      <div class="sidebar__links">
        <div class="sidebar__link"
             v-scroll-to="{el: '#welcome', duration: 700, offset: -100}"
             @click="sidebarOpen = false">Главная</div>
        <div class="sidebar__link"
             v-scroll-to="{el: '#services', duration: 700, offset: -100}"
             @click="sidebarOpen = false">Услуги</div>
        <div class="sidebar__link"
             v-scroll-to="{el: '#bitrix', duration: 700, offset: -100}"
             @click="sidebarOpen = false">Битрикс24</div>
        <div class="sidebar__link"
             v-scroll-to="{el: '#steps', duration: 700, offset: -100}"
             @click="sidebarOpen = false">Заявка</div>
        <div class="sidebar__link"
             v-scroll-to="{el: '#contact', duration: 700, offset: -100}"
             @click="sidebarOpen = false">Контакты</div>
      </div>

      <div class="sidebar__socials">
        <a href="#" class="sidebar__social">
          <svg width="20" height="20">
            <use href="../assets/img/icons.svg#footer-inst"></use>
          </svg>
        </a>

        <a href="#" class="sidebar__social">
          <svg width="20" height="20">
            <use href="../assets/img/icons.svg#footer-fb"></use>
          </svg>
        </a>
      </div>

      <div class="sidebar__call-box">
        <a href="tel: +7 (777) 205 93 39" class="sidebar__phone-text">
          +7 (777) 2059339
        </a>
        <a href="" class="sidebar__call-order"
           v-scroll-to="{el: '#contact', duration: 700, offset: -100}"
           @click="sidebarOpen = false">
          Заказать обратный звонок
        </a>
      </div>

      <div class="sidebar__mail-box">

        <svg width="56" height="56">
          <use href="../assets/img/icons.svg#mail-box"></use>
        </svg>

        <div class="sidebar__mail-info">
          <h6>
            Напишите нам
          </h6>
          <p>
            info@jasan.kz
          </p>
        </div>

      </div>

    </div>

  </header>
</template>

<script>
export default {
  data() {
    return {
      sidebarOpen: false
    };
  },
  methods: {
    linker(link) {
      window.open(link, '_blank')
      //window.location = "https://www.bitrix24.kz/create.php?p=13670906"
    },
  }
};
</script>

<style lang="scss" scoped>

</style>
