<template>
  <div>
    <div class="container-sm text-center py-5">
      <h2 class="pb-3">Some Brands We Work With</h2>
      <p class="pb-3">Lorem ipsum dolor sit amet consectetur adipisicing.</p>
      <div class="row pt-4">
        <div v-for="brand in brands" :key="brand.id" class="col-sm-2">
          <img
            class="w-50"
            :src="require(`../assets/img/${brand.path}`)"
            :alt="brand.id"
          />
        </div>
      </div>
      <div class="row_sandy p-2 row align-items-center justify-content-between">
        <div class="col-auto">
          <div class="d-flex flex-row align-items-center gap-3">
            <div class="wrapper_img">
              <img
                class="rounded-circle w-100"
                src="@/assets/img/marketing-expert-cta.png"
                alt="Sandy Reiff"
              />
            </div>
            <div class="d-flex flex-column text-start">
              <h5>Sandy Reiff</h5>
              <p class="sandy_info">Marketing Consultant Expert</p>
            </div>
          </div>
        </div>
        <div class="col-auto">
          <h4>Drive Leads and Sales with Avada</h4>
        </div>
        <div class="col-auto d-inline-block pe-3">
          <button class="btn">
            <font-awesome-icon icon="fa-solid fa-phone" class="pe-2" />
            (555) 802-1234
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import brands from "@/assets/data/brands";

export default {
  name: "GeneralBrands",
  data() {
    return {
      brands,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

h2 {
  font-size: 50px;
  font-weight: 700;
}

button {
  @include button($color-Ecstasy-Op, $color-Ecstasy, $color-Ecstasy, white);
}

.row_sandy {
  margin-top: 100px;
  border-radius: 5px;
  box-shadow: 0px 10px 30px 10px rgba($color-Gunsmoke, 0.5);

  .wrapper_img {
    width: 50px;
  }

  .sandy_info {
    font-size: 12px;
  }
}
</style>