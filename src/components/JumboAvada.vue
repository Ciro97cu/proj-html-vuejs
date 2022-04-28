<template>
  <div id="jumbo" class="py-3">
    <div class="container-sm">
      <div class="row align-items-center justify-content-between">
        <div class="col-sm-6 text-white">
          <h1 class="pb-4">Unlock Your Online Growth Potential</h1>
          <p class="pb-4">
            Online Marketing to secure customer retention, leads, and sales. We
            focus on the bigger picture.
          </p>
          <button class="btn border border-white">
            Our Services
            <font-awesome-icon icon="fa-solid fa-arrow-right" class="ps-2" />
          </button>
        </div>
        <MarketingExpertCard />
      </div>
    </div>
    <div id="special_div">
      <div class="mb-2 p-2 bg-white d-flex flex-column align-items-center">
        <font-awesome-icon icon="fa-solid fa-mountain" class="fa-2x" />
        <p class="pt-1 text_bottom">Demos</p>
      </div>
      <div class="mb-2 p-2 bg-white d-flex flex-column align-items-center">
        <p>
          <span><sup>$</sup>39</span>
        </p>
        <p class="text_bottom">On Sale</p>
      </div>
    </div>
  </div>
</template>

<script>
import MarketingExpertCard from "./MarketingExpertCard.vue";

export default {
  name: "JumboAvada",
  components: {
    MarketingExpertCard,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

#jumbo {
  background-image: url(../assets/img/marketing-intro.jpg);
  background-size: cover;
  position: relative;

  #special_div {
    position: absolute;
    top: 2em;
    right: 2em;

    & > div {
      border-radius: 10px;
    }

    span {
      color: rgb(97, 201, 97);
      font-size: 30px;
      font-weight: 700;
    }

    .text_bottom {
      font-weight: 500;
    }
  }

  .row {
    min-height: 600px;
    position: relative;

    .col-sm-6 {
      h1 {
        font-size: 50px;
        font-weight: 700;
      }

      p {
        font-size: 25px;
      }

      button {
        @include button(white, black, transparent, white);
      }
    }
  }
}
</style>