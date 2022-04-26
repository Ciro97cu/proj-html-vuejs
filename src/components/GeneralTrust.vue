<template>
  <div>
    <div class="container-sm py-5">
      <h2 class="text-center pb-5">Trusted by Leading Organizations</h2>
      <div class="row pb-5">
        <div class="col-sm-4" v-for="person in trust" :key="person.id">
          <img
            class="w-100 pb-4"
            :src="require(`../assets/img/${person.path}`)"
            :alt="person.id"
          />
          <h4 class="pb-4">{{ person.title }}</h4>
          <h3 class="pb-2">{{ person.value }}</h3>
          <p>{{ person.info }}</p>
        </div>
      </div>
      <div class="row justify-content-center">
        <button class="btn col-auto">Read More Case Studies</button>
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