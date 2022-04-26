<template>
  <div>
    <div class="container-sm pb-5">
      <h3 class="text-center pb-4">Awards</h3>
      <div class="row">
        <div
          class="col-sm-3 d-flex flex-column align-items-center"
          v-for="award in awards"
          :key="award.id"
        >
          <img
            class="w-25 pb-2"
            :src="require(`../assets/img/${award.path}`)"
            :alt="award.id"
          />
          <p class="text-center">{{ award.text }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import awards from "@/assets/data/awards";

export default {
  name: "AwardsAvada",
  data() {
    return {
      awards,
    };
  },
};
</script>

<style lang="scss" scoped>
h3 {
  font-weight: 700;
}
</style>