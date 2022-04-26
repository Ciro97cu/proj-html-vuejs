<template>
  <div>
    <NavAvada class="bg-white" :arrayNav="arrayNav" />
    <JumboAvada />
  </div>
</template>

<script>
import NavAvada from "./NavAvada.vue";
import JumboAvada from "./JumboAvada.vue";

export default {
  name: "HeaderAvada",
  components: {
    NavAvada,
    JumboAvada,
  },
  data() {
    return {
      arrayNav: [
        {
          name: "Home",
          dropdown: true,
        },
        {
          name: "Services",
          dropdown: true,
        },
        {
          name: "Why US",
          dropdown: false,
        },
        {
          name: "Case Studies",
          dropdown: false,
        },
        {
          name: "About",
          dropdown: false,
        },
        {
          name: "Blog",
          dropdown: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
</style>