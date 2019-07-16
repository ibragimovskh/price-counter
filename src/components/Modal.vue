<template>
  <div>
    <!-- eslint-disable -->
    <b-modal v-for="modal in modals" :id="modal.id" :title="modal.title" :key="modal.id" size="xl">
      <span>Данный расчет не даёт точной оценки, но позволяет определить общий бюджет и нижнюю границу стоимости разработки сайта.</span>
    </b-modal>
  </div>
</template>

<script>
export default {
  data() {
    return {
      modals: [
        {
          id: "landing",
          title: "Landing Page"
        },
        { id: "business", title: "Бизнес-сайт" },
        { id: "store", title: "Интернет Магазин" }
      ]
    };
  }
};
</script>