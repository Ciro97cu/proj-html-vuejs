<template>
  <main>
    <IntroductionSection />
    <PlanSection />
    <TeamSection />
    <MarketingSection />
    <ContactSection />
  </main>
</template>

<script>
import IntroductionSection from "./IntroductionSection.vue";
import PlanSection from "./PlanSection.vue";
import TeamSection from "./TeamSection.vue";
import MarketingSection from "./MarketingSection.vue";
import ContactSection from "./ContactSection.vue";

export default {
  name: "MainAvada",
  components: {
    IntroductionSection,
    PlanSection,
    TeamSection,
    MarketingSection,
    ContactSection,
  },
};
</script>

<style lang="scss" scoped>
</style>