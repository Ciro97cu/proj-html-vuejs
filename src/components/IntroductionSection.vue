<template>
  <div>
    <GeneralInfo />
    <GeneralBrands />
    <GeneralTrust />
  </div>
</template>

<script>
import GeneralInfo from "./GeneralInfo.vue";
import GeneralBrands from "./GeneralBrands.vue";
import GeneralTrust from "./GeneralTrust.vue";

export default {
  name: "IntroductionSection",
  components: {
    GeneralInfo,
    GeneralBrands,
    GeneralTrust,
  },
};
</script>

<style lang="scss" scoped>
</style>