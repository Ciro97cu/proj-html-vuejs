<template>
  <div id="app">
    <HeaderAvada />
    <MainAvada />
    <FooterAvada />
  </div>
</template>

<script>
import HeaderAvada from "./components/HeaderAvada.vue";
import MainAvada from "./components/MainAvada.vue";
import FooterAvada from "./components/FooterAvada.vue";

export default {
  name: "App",
  components: {
    HeaderAvada,
    MainAvada,
    FooterAvada,
  },
};
</script>

<style lang="scss">
@import "./assets/style/import.scss";
@import "./assets/style/resets.scss";
@import "./assets/style/variables.scss";

*::-webkit-scrollbar {
  width: 12px;
}
*::-webkit-scrollbar-track {
  background: white;
}
*::-webkit-scrollbar-thumb {
  background-color: $color-Ecstasy-Op;
  border-radius: 20px;
}
*::-webkit-scrollbar-thumb:hover {
  background: $color-Ecstasy;
}
</style>
