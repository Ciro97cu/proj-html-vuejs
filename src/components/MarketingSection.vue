<template>
  <div id="marketing_section">
    <div class="container-sm py-5">
      <div class="row py-5">
        <div class="col-sm-6">
          <h2>
            Marketing Resources: Insider Advice on How to Increase Online Sales
          </h2>
        </div>
        <div class="col-sm-6 align-self-end text-end">
          <button class="btn">Explore All Resources</button>
        </div>
      </div>

      <div class="row py-5">
        <div class="col-sm-4" v-for="card in marketing" :key="card.id">
          <img
            class="w-100 pb-4"
            :src="require(`../assets/img/${card.path}`)"
            :alt="card.id"
          />
          <h3>{{ card.text }}</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import marketing from "@/assets/data/marketing";

export default {
  name: "MarketingSection",
  data() {
    return {
      marketing,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

#marketing_section {
  background-color: $color-Gray-Nurse;

  h2 {
    max-width: 70%;
    font-weight: 700;
  }

  button {
    @include button($color-Ecstasy, white, $color-Tango, black);
  }

  h3 {
    font-weight: 600;
  }
}
</style>