<template>
  <div>
    <!-- eslint-disable -->
    <b-modal id="landing" title="Landing Page" size="xl">
      <b-container>
        <b-row>
          <b-col>
            <h3 class="modal__title">Модули:</h3>
            <b-form-group>
              <b-form-checkbox-group v-model="landing.price">
                <b-form-checkbox
                  v-for="module in landing.modules"
                  :value="module.price"
                  :key="module.name"
                  v-model="landing.selected"
                >{{landing.selected}}</b-form-checkbox>
              </b-form-checkbox-group>
            </b-form-group>
            {{countPrice}}
          </b-col>
        </b-row>
      </b-container>
    </b-modal>
    <b-modal id="business" title="Бизнес-сайт" size="xl">
      <b-container>
        <b-row></b-row>
      </b-container>
    </b-modal>
    <b-modal id="store" title="Интернет Магазин" size="xl">
      <b-container>
        <b-row></b-row>
      </b-container>
    </b-modal>
  </div>
</template>

<script>
export default {
  data() {
    return {
      landing: {
        modules: [
          {
            name: "Галерея",
            price: 1500
          },
          {
            name: "Слайдер",
            price: 2000
          },
          {
            name: "Поиск",
            price: 3000
          },
          {
            name: "Обратный звонок",
            price: 4000
          },
          {
            name: "Хостинг",
            price: 4200
          },
          {
            name: "Форма обратной связи",
            price: 2100
          }
        ],
        selected: [false, false, false, false, false, false]
      }
    };
  },
  computed: {
    countPrice() {
      return this.landing.selected.reduce((a, b) => a + b);
    }
  }
};
</script>