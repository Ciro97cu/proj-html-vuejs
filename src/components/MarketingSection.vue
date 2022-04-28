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
          <div class="wrapper_img">
            <img
              class="w-100 h-100"
              :src="require(`../assets/img/${card.path}`)"
              :alt="card.id"
            />
            <div class="filter_img"></div>
          </div>
          <h3 class="pt-4">{{ card.text }}</h3>
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

  .wrapper_img {
    @include imgHover($color-Ecstasy, 4/3);
  }

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