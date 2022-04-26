<template>
  <main>
    <IntroductionSection />
    <PlanSection />
    <TeamSection />
  </main>
</template>

<script>
import IntroductionSection from "./IntroductionSection.vue";
import PlanSection from "./PlanSection.vue";
import TeamSection from "./TeamSection.vue";

export default {
  name: "MainAvada",
  components: {
    IntroductionSection,
    PlanSection,
    TeamSection,
  },
};
</script>

<style lang="scss" scoped>
</style>