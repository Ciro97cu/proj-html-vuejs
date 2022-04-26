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
        <div class="col-sm-5"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumboAvada",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

#jumbo {
  background-image: url(../assets/img/marketing-intro.jpg);
  background-size: cover;

  .row {
    min-height: 700px;

    .col-sm-6 {
      h1 {
        font-size: 50px;
        font-weight: 700;
      }

      p {
        font-size: 25px;
      }

      button {
        @include button(white, black, transparent);
      }
    }
  }
}
</style>