<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";

export default {
  name: "FooterAvada",
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>

<style lang="scss" scoped>
</style>