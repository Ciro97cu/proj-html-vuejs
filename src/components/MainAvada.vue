<template>
  <main>
    <IntroductionSection />
    <PlanSection />
  </main>
</template>

<script>
import IntroductionSection from "./IntroductionSection.vue";
import PlanSection from "./PlanSection.vue";
export default {
  name: "MainAvada",
  components: {
    IntroductionSection,
    PlanSection,
  },
};
</script>

<style lang="scss" scoped>
</style>