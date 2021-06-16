<template>
  <main class="main">
    <section class="main__section welcome-section" :style="{ 'background-image': randomBg}" id="welcome">
      <div class="welcome-section__container">
        <h1 class="welcome-section__heading">
          <span>Автоматизируй</span> <br>
          свой бизнес
        </h1>

        <p class="welcome-section__subtitle">
          Проследи путь, который совершает клиент с момента, <br>
          когда он только узнал о товаре и до покупки.
        </p>

        <button class="welcome-section__btn button" v-scroll-to="{el: '#services', duration: 700, offset: -160}">
          Подробнее
        </button>
      </div>
    </section>

    <section class="main__section company-slider">
      <div class="company-slider__container">
        <div class="company-slider__title title-small">
          Наши партнеры
        </div>

        <div class="company-slider__heading heading-medium">
          Встречайте наших партнеров
        </div>

        <div class="company-slider__wrapper">

          <div class="swiper-container company-slider__swiper-container">

            <div class="swiper-wrapper company-slider__inner-wrapper">
              <div class="swiper-slide company-slider__item" @click="linker(`https://www.bloomzed.kz`)" >
                <img src="../assets/img/bloomzed.png" alt="" class="company-slider__img">
              </div>

              <div class="swiper-slide company-slider__item" @click="linker(`https://100potolkov.kz/`)">
                <img src="../assets/img/100-potolkov.png" alt="" class="company-slider__img">
              </div>

              <div class="swiper-slide company-slider__item" @click="linker(`https://100za5.kz/`)">
                <img src="../assets/img/100za5.jpg" alt="" class="company-slider__img">
              </div>

              <div class="swiper-slide company-slider__item" @click="linker(`http://www.kings-speech.kz/`)">
                <img src="../assets/img/king-speech.jpg" alt="" class="company-slider__img">
              </div>

              <div class="swiper-slide company-slider__item" @click="linker(`https://immuneplusworld.com/`)">
                <img src="../assets/img/immune.png" alt="" class="company-slider__img">
              </div>

              <div class="swiper-slide company-slider__item">
                <img src="../assets/img/unie.png" alt="" class="company-slider__img">
              </div>
            </div>

          </div>

          <div class="company-slider__next" @click="nextSlideCompany"></div>
          <div class="company-slider__prev" @click="prevSlideCompany"></div>

        </div>

      </div>
    </section>

    <section class="main__section about-section">

      <div class="about-section__container">

        <div class="about-section__info">
          <div class="about-section__title title-small">
            Кто мы?
          </div>

          <div class="about-section__heading heading-medium">
            Узнайте о нас больше и станьте нашим клиентом
          </div>

          <div class="about-section__text">
            Компания "Jasan" специализируется на комплексной автоматизации бизнеса. Рады предложить вам различные форматы решений вашего запроса для совместного достижения желаемых результатов.
            <br><br>
            Наша миссия — помогать бизнесу работать эффективнее. Для этого мы внедряем современное ПО и модернизируем ИТ-сервисы. Сотрудничаем с клиентами по принципу «одного окна»: оказываем максимальный спектр услуг внедрения, эксплуатации и поддержки ИТ для бизнеса.
          </div>
        </div>

        <div class="about-section__achieves">

          <div class="about-section__item about-section__item--1">
            <svg class="about-section__icon" width="89" height="80">
              <use href="../assets/img/icons.svg#document"></use>
            </svg>

            <div class="about-section__item-title">
              250+
            </div>

            <div class="about-section__item-subtitle">
              Счастливые клиенты
            </div>
          </div>

          <div class="about-section__item about-section__item--2">
            <svg class="about-section__icon" width="89" height="80">
              <use href="../assets/img/icons.svg#document"></use>
            </svg>

            <div class="about-section__item-title">
              10+
            </div>

            <div class="about-section__item-subtitle">
              Лет опыт работы
            </div>
          </div>

          <div class="about-section__item about-section__item--3">
            <svg class="about-section__icon" width="89" height="80">
              <use href="../assets/img/icons.svg#document"></use>
            </svg>

            <div class="about-section__item-title">
              300+
            </div>

            <div class="about-section__item-subtitle">
              Успешный проекты
            </div>
          </div>

        </div>

      </div>

    </section>

    <section class="main__section tariff-section" id="services">

      <div class="tariff-section__container">

        <div class="tariff-section__title title-small">Наши пакеты</div>
        <div class="tariff-section__heading heading-medium">С нами все проще</div>
        <div class="tariff-section__subtitle">
          Приобретите Битрикс24 у нас и получите бесплатные часы внедрения, неограниченную поддержку. Уже более 1000 компаний работают эффективнее с Битрикс24 благодаря нам.
        </div>

        <div class="tariff-section__list">

          <div class="tariff-section__item tariff-card">
            <div class="tariff-card__top">
              <svg class="tariff-card__icon" width="102" height="102">
                <use href="../assets/img/icons.svg#book"></use>
              </svg>

              <div class="tariff-card__name">
                Начальный
              </div>

              <ul class="tariff-card__list">
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
              </ul>
            </div>

            <div class="tariff-card__bottom">
              <div class="tariff-card__price">
                от <span>50 000 тг.</span>
              </div>


              <button class="tariff-card__btn button button--outline" v-scroll-to="{el: '#contact', duration: 700, offset: -160}" @click="preText(`Начальный`)">
                Заказать
              </button>
            </div>
          </div>

          <div class="tariff-section__item tariff-card">
            <div class="tariff-card__top">
              <svg class="tariff-card__icon" width="102" height="102">
                <use href="../assets/img/icons.svg#target"></use>
              </svg>

              <div class="tariff-card__name" v-scroll-to="{el: '#contact', duration: 700, offset: -160}">
                Стандартный
              </div>

              <ul class="tariff-card__list">
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
              </ul>
            </div>

            <div class="tariff-card__bottom">
              <div class="tariff-card__price">
                от <span>90 000 тг.</span>
              </div>

              <button class="tariff-card__btn button button--outline" v-scroll-to="{el: '#contact', duration: 700, offset: -160}" @click="preText(`Стандартный`)">
                Заказать
              </button>
            </div>
          </div>

          <div class="tariff-section__item tariff-card tariff-card--accent">
            <div class="tariff-card__top">
              <svg class="tariff-card__icon" width="102" height="102">
                <use href="../assets/img/icons.svg#flag"></use>
              </svg>

              <div class="tariff-card__name">
                Улучшенный
              </div>

              <ul class="tariff-card__list">
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
              </ul>
            </div>

            <div class="tariff-card__bottom">
              <div class="tariff-card__price">
                от <span>120 000 тг.</span>
              </div>

              <button class="tariff-card__btn button button--outline" v-scroll-to="{el: '#contact', duration: 700, offset: -160}" @click="preText(`Улучшенный`)">
                Заказать
              </button>
            </div>
          </div>

          <div class="tariff-section__item tariff-card">
            <div class="tariff-card__top">
              <svg class="tariff-card__icon" width="102" height="102">
                <use href="../assets/img/icons.svg#rocket"></use>
              </svg>

              <div class="tariff-card__name">
                Продвинутый
              </div>

              <ul class="tariff-card__list">
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                <li class="tariff-card__item">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
              </ul>
            </div>

            <div class="tariff-card__bottom">
              <div class="tariff-card__price">
                от <span>160 000 тг.</span>
              </div>

              <button class="tariff-card__btn button button--outline" v-scroll-to="{el: '#contact', duration: 700, offset: -160}" @click="preText(`Продвинутый`)">
                Заказать
              </button>
            </div>
          </div>

        </div>
      </div>

    </section>

    <section class="main__section bitrix-section" id="bitrix">

      <div class="bitrix-section__container">

        <div class="bitrix-section__title title-small">
          Bitrix24
        </div>

        <div class="bitrix-section__row">
          <h2 class="bitrix-section__heading heading-medium">
            Быстро, просто, эффективно
          </h2>

          <button class="bitrix-section__btn button" @click="linker(`https://www.bitrix24.kz/create.php?p=13670906`)">
            Перейти в Битрикс
          </button>
        </div>

        <div class="bitrix-section__list">

          <div class="bitrix-section__item">
            <div class="bitrix-section__name">
              CRM
            </div>

            <div class="bitrix-section__text">
              Бесплатный онлайн-офис позволяет организовать работу всех отделов компании, координировать и отслеживать эффективность каждого сотрудника. Подключение IP-телефонии, почты и всех мессенджеров в контакт-центр позволяет обрабатывать все поступающие обращения в рамках одного интерфейса
            </div>
          </div>

          <div class="bitrix-section__item">
            <div class="bitrix-section__name">
              Задачи и проекты
            </div>

            <div class="bitrix-section__text">
              Система автоматически продвигает клиента по этапам сделки в воронке и регистрирует данные в CRM-карточку. Встроенное защищенное хранилище предполагает удобную работу со всеми документами компании с возможностью настройки прав на доступ.
            </div>
          </div>

          <div class="bitrix-section__item">
            <div class="bitrix-section__name">
              Онлайн оффис
            </div>

            <div class="bitrix-section__text">
              Система автоматически фиксирует все поступающие задачи и напоминает сотрудникам о сроках и выполнения. Встроенный конструктор позволяет быстро подключить Яндекс.Метрику и Google.Analytics, и создать магазин с прямой интеграцией в CRM.
            </div>
          </div>

        </div>

      </div>
    </section>

    <section class="main__section steps-section" id="steps">
      <div class="steps-section__container">

        <div class="steps-section__title title-small">
          Шаги
        </div>

        <h2 class="steps-section__heading heading-medium">
          Несколько шагов до успеха
        </h2>

        <div class="steps-section__subtitle">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vitae lectus sit cras libero. Sit nunc potenti id
          iaculis. Mi odio sit integer sit vel porttitor vestibulum sit donec.
        </div>

        <div class="steps-section__list">

          <div class="steps-section__step" v-for="i in this.arraySteps">

            <div class="steps-section__info">
              <div class="steps-section__name">
                Шаг {{ i.id }}. {{i.name}}
              </div>
              <div class="steps-section__text">
                 {{i.desc}}
              </div>
            </div>

            <div class="steps-section__icon">
              <svg width="89" height="81">
                <use href="../assets/img/icons.svg#document"></use>
              </svg>
            </div>

          </div>


        </div>

      </div>
    </section>

    <section class="main__section contact-section" id="contact">

      <div class="contact-section__container">

        <div class="contact-section__title title-small">
          Контакты
        </div>

        <div class="contact-section__heading heading-medium">
          Свзязаться с нами
        </div>

        <form class="contact-section__form">
          <input type="text"
                 class="contact-section__input input"
                 placeholder="Имя"
                 v-model="name"
                 :class="{'input--error' : nameStatus}">

          <input type="email"
                 class="contact-section__input input"
                 placeholder="Адрес электронной почти"
                 v-model="email"
                 :class="{'input--error' : emailStatus}">

          <input type="tel"
                 class="contact-section__input input"
                 placeholder="Телефон"
                 v-model="phoneNumber"
                 id="phoneNumber"
                 :class="{'input--error' : phoneStatus}">

          <textarea class="contact-section__textarea input input--textarea"
                    placeholder="Напишите свое сообщение сюда..."
                    v-model="message"
                    :class="{'input--error' : messageStatus}"></textarea>
          <!--
          <label class="contact-section__policy-box">
            <input type="checkbox" class="contact-section__checkbox" v-model="policy">
            <span class="contact-section__checkmark"></span>

            <span class="contact-section__policy-text">
                Я согласен(а) с <a href="#">политика конфиденциальности</a>
            </span>
          </label> -->

          <div class="contact-section__error">
            {{ errorMessage }}
          </div>

          <button class="contact-section__btn button" @click.prevent="sendForm">
            Отправить
          </button>

        </form>

      </div>

      <img src="../assets/img/contact-img.png" alt="" class="contact-section__img">
    </section>

    <div class="modal" v-if="modalStatus">

      <div class="modal__wrapper">

        <img src="../assets/img/icons/modal-check-2.png" alt="" class="modal__checkmark">

        <div class="modal__text">
          Ваша заявка успешно отправлена. <br>
          С вами свяжутся в ближайшее время
        </div>

        <button class="modal__btn button" @click="modalStatus = false">
          Круто!
        </button>

      </div>

    </div>

  </main>
</template>

<script>
import allBackgroundImages from '../assets/bg-set/onLoadBg'
import Swiper, {Pagination, Autoplay, Navigation} from 'swiper';
import IMask from 'imask'

Swiper.use([Pagination, Autoplay, Navigation]);

export default {
  data() {
    return {
      arraySteps: [
        {id: 1, name: "Предпроектный анализ", desc: "Предпроектный анализ"},
        {id: 2, name: "Регистрация облачного портала", desc: "Регистрация облачного портала"},
        {id: 3, name: "Настройка поддомена", desc: "Настройка поддомена"},
        {id: 4, name: "Базовые настройки системы", desc: "Базовые настройки системы"},
        {id: 5, name: "Создание структуры компании в Битрикс24", desc: "Создание структуры компании в Битрикс24"},
        {id: 6, name: "Добавление пользователей на портал", desc: "Добавление пользователей на портал"},
        {id: 7, name: "Распределение пользователей по структуре", desc: "Распределение пользователей по структуре"},

        ],
      allBackgroundImages,
      companySwiper: null,
      name: '',
      email: '',
      phoneNumber: '',
      message: '',
      policy: false,
      errorMessage: '',
      nameStatus: false,
      phoneStatus: false,
      emailStatus: false,
      messageStatus: false,
      modalStatus: false
    }
  },
  computed: {
    randomBg() {
      const randIndex = Math.floor(Math.random() * this.allBackgroundImages.length)
      return `url(${this.allBackgroundImages[randIndex]})`
    }
  },
  methods: {
    nextSlideCompany() {
      this.companySwiper.slideNext()
    },
    prevSlideCompany() {
      this.companySwiper.slidePrev()
    },
    linker(link) {
      window.open(link, '_blank')
      //window.location = "https://www.bitrix24.kz/create.php?p=13670906"
    },
    preText(text) {
      this.message = `Добрый день! Хотели бы поподробнее узнать о тарифе "` +  text + `", не могли бы нас проконсультировать.`
    },
    sendForm() {
      if (this.policy === false) {
        this.errorMessage = 'Пожалуйста, ознакомьтесь с политикой конфиденциальности'
      }

      if (this.name === '') {
        this.errorMessage = 'Пожалуйста, заполните все поля'
        this.nameStatus = true
      } else {
        this.nameStatus = false
      }

      if (this.email === '') {
        this.errorMessage = 'Пожалуйста, заполните все поля'
        this.emailStatus = true
      } else {
        this.emailStatus = false
      }

      if (this.phoneNumber === '') {
        this.errorMessage = 'Пожалуйста, заполните все поля'
        this.phoneStatus = true
      } else {
        this.phoneStatus = false
      }

      if (this.message === '') {
        this.errorMessage = 'Пожалуйста, заполните все поля'
        this.messageStatus = true
      } else {
        this.messageStatus = false
      }

      const params = new URLSearchParams()
      params.append('name', this.name)
      params.append('phoneNumber', this.phoneNumber)
      params.append('comment', this.message)
      params.append('email', this.email)

      const config = {
        headers: {
          'Content-Type': 'application/x-www-form-urlencoded'
        }
      }

      if (this.policy && this.name !== '' && this.email !== '' && this.phoneNumber !== '' && this.message !== '') {
        this.errorMessage = ''

        this.$axios.post(process.env.API_URL + 'email', params, config)
          .then(response => {
            console.log(response)
            this.name = ''
            this.phoneNumber = ''
            this.message = ''
            this.email = ''
            this.modalStatus = true
          })
          .catch(e => console.log(e))
      }
    }
  },
  mounted() {
    var inputMask = document.getElementById('phoneNumber');
    var maskOptions = {
      mask: '+{7}(000)000-00-00'
    };
    var mask = IMask(inputMask, maskOptions);
    mask.updateValue();

    this.companySwiper = new Swiper('.company-slider__swiper-container', {
      slidesPerView: 1,
      spaceBetween: 8,
      loop: true,
      breakpoints: {
        768: {
          slidesPerView: 3,
          spaceBetween: 20,
        },
        1140: {
          slidesPerView: 5,
          spaceBetween: 40,
        }
      }
    });
  }
}
</script>

<style>

</style>
