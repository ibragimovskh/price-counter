<template>
  <div id="app">
    <Header/>
    <Services/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Services from "./components/Services.vue";

export default {
  name: "app",
  components: {
    Header: Header,
    Services: Services
  }
};
</script>

<style lang="scss">
@import "node_modules/bootstrap/scss/bootstrap-reboot.scss";
@import "node_modules/bootstrap/scss/bootstrap.scss";
@import "node_modules/bootstrap-vue/dist/bootstrap-vue.scss";
@import "src/assets/main.scss";
</style>
