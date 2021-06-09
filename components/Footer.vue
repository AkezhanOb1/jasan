<template>
  <footer class="footer">
    <div class="footer__container">

      <div class="footer__logo-box" v-scroll-to="{el: '#welcome', duration: 700, offset: -140}">
        <img src="../assets/img/logo-jasan.png" alt="" class="footer__logo">

        <div class="footer__grey-text">
          Самые эффективные CRM <br>
          услуги в Казахстане
        </div>

      </div>

      <div class="footer__link-box">

        <div class="footer__links">
          <div class="footer__link" v-scroll-to="{el: '#welcome', duration: 700, offset: -140}">Главная</div>
          <div class="footer__link" v-scroll-to="{el: '#services', duration: 700, offset: -160}">Услуги</div>
          <div class="footer__link" v-scroll-to="{el: '#bitrix', duration: 700, offset: -160}">Битрикс24</div>
        </div>

        <div class="footer__links">
          <div class="footer__link" v-scroll-to="{el: '#steps', duration: 700, offset: -160}">Заявка</div>
          <div class="footer__link" v-scroll-to="{el: '#contact', duration: 700, offset: -160}">Контакты</div>
        </div>

      </div>

      <div class="footer__contacts">

        <div class="footer__contact-box">

          <svg class="footer__icon" width="19" height="13">
            <use href="../assets/img/icons.svg#mail"></use>
          </svg>

          <div class="footer__contact-text">
            info@jasan.kz
          </div>

        </div>

        <div class="footer__contact-box">

          <svg class="footer__icon" width="16" height="16">
            <use href="../assets/img/icons.svg#phone"></use>
          </svg>

          <div class="footer__phone-group">
            <a href="tel: +7 (777) 205 93 39" class="footer__contact-text footer__contact-text--mb10">
              +7 (777) 2059339
            </a>

            <a href="tel: +7 (777) 205 93 39" class="footer__contact-text">
              +7 (777) 2059339
            </a>
          </div>

        </div>

        <div class="footer__contact-box">

          <svg class="footer__icon" width="20" height="20">
            <use href="../assets/img/icons.svg#map-pin"></use>
          </svg>

          <div class="footer__contact-text" @click="linker(`https://go.2gis.com/7hc23`)">
            Алматы, Алмалинский район, <br>
            Айтеке би 187, офис 216
          </div>

        </div>

      </div>

      <div class="footer__social-box">
        <div class="footer__social-title">
          мы в социальных сетях
        </div>

        <div class="footer__socials">
          <a class="footer__social">
            <svg width="20" height="20" @click="linker(`https://www.facebook.com/jasankz/`)">
              <use href="../assets/img/icons.svg#footer-fb"></use>
            </svg>
          </a>
          <a class="footer__social">
            <svg width="20" height="20" @click="linker(`https://www.instagram.com/jasan_technologies/`)">
              <use href="../assets/img/icons.svg#footer-inst"></use>
            </svg>
          </a>
        </div>

        <div class="footer__privacy-text">
          © Jasan. LTD, 2021. <br>
          Все права зашищены
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  methods: {
    linker(link) {
      window.open(link, '_blank')
      //window.location = "https://www.bitrix24.kz/create.php?p=13670906"
    },
  }
};
</script>
