<template>
  <div>
    <div class="container-sm py-5">
      <h2 class="text-center">Trusted by Leading Organizations</h2>
      <div class="row pb-5">
        <div class="col-sm-4" v-for="person in trust" :key="person.id">
          <div v-if="person.toggle">
            <div class="wrapper_img mt-5">
              <img
                class="w-100 h-100"
                :src="require(`../assets/img/${person.path}`)"
                :alt="person.id"
              />
              <div class="filter_img"></div>
            </div>
            <h4 class="py-4">{{ person.title }}</h4>
            <h3 class="pb-2">{{ person.value }}</h3>
            <p>{{ person.info }}</p>
          </div>
        </div>
      </div>
      <div class="row justify-content-center pb-5">
        <button class="btn col-auto" @click="displayMore()">
          Read More Case Studies
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import trust from "@/assets/data/trust";

export default {
  name: "GeneralTrust",
  data() {
    return {
      trust,
    };
  },
  methods: {
    displayMore: function () {
      console.log(trust);
      for (let i = 3; i < 6; i++) {
        trust[i].toggle = !trust[i].toggle;
      }
    },
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

.col-sm-4 {
  .wrapper_img {
    @include imgHover($color-Ecstasy, 2/3);
  }

  h4 {
    font-size: 25px;
  }
  h3 {
    font-size: 40px;
    font-weight: 700;
  }
}

button {
  @include button($color-Ecstasy, white, $color-Tango, black);
}
</style>