<template>
  <div>
    <NavAvada class="bg-white" />
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
};
</script>

<style lang="scss" scoped>
</style>