<template>
  <section class="services">
    <b-container>
      <h3 class="services__title text-center mb-5 text-uppercase font-weight-bold">Услуги</h3>
      <b-row>
        <b-col class="services__card p-5 text-center border-right" lg="4" md="6" sm="12">
          <h4 class="services__card-title">Landing Page</h4>
          <p class="services__card-text pt-4 pb-4">
            Основная задача Landing Page это продажи товара или услуги с максимальным результатом!
            Landing Page подходит для любых товаров или услуг.
          </p>
          <b-button class="services__card-button" v-b-modal.landing>РАСЧИТАТЬ СТОИМОСТЬ САЙТА</b-button>
        </b-col>
        <b-col class="services__card p-5 text-center border-right" lg="4" md="6" sm="12">
          <h4 class="services__card-title">Бизнес-сайт</h4>
          <p
            class="services__card-text pt-4 pb-4"
          >Поможет предоставить пользователю всю информацию о деятельности компании, товарах или услугах для расширения рынка сбыта продукции или привлечения партнёров.</p>
          <b-button class="services__card-button" v-b-modal.business>РАСЧИТАТЬ СТОИМОСТЬ САЙТА</b-button>
        </b-col>
        <b-col class="services__card p-5 text-center" lg="4" md="12" sm="12">
          <h4 class="services__card-title">Интернeт магазин</h4>
          <p
            class="services__card-text pt-4 pb-4"
          >Удобное и простое совершение покупки в Интернет-магазине наша главная цель! Наши Интернет-магазины справляются с основными задачами с наивысшим результатом!</p>
          <b-button class="services__card-button" v-b-modal.store>РАСЧИТАТЬ СТОИМОСТЬ САЙТА</b-button>
        </b-col>
        <!-- MODALS -->
        <Modal />
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Modal from "./Modal";

export default {
  data() {
    return {};
  },
  methods: {},
  components: {
    Modal: Modal
  }
};
</script>
