<template>
  <div id="plan_container">
    <WorkWithus />
    <AwardsAvada />
  </div>
</template>

<script>
import WorkWithus from "./WorkWithus.vue";
import AwardsAvada from "./AwardsAvada.vue";

export default {
  name: "PlanSection",
  components: {
    WorkWithus,
    AwardsAvada,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

#plan_container {
  background-color: $color-Gray-Nurse;
}
</style>