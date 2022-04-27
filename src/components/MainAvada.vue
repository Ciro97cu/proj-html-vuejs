<template>
  <main>
    <IntroductionSection />
    <PlanSection />
    <TeamSection />
    <MarketingSection />
  </main>
</template>

<script>
import IntroductionSection from "./IntroductionSection.vue";
import PlanSection from "./PlanSection.vue";
import TeamSection from "./TeamSection.vue";
import MarketingSection from "./MarketingSection.vue";

export default {
  name: "MainAvada",
  components: {
    IntroductionSection,
    PlanSection,
    TeamSection,
    MarketingSection,
  },
};
</script>

<style lang="scss" scoped>
</style>