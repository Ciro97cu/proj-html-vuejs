<template>
  <div>
    <div class="container-sm py-5">
      <div class="row py-5">
        <div class="col-sm-6">
          <h2 class="pb-4">
            Grow Your Online Business Strategically, and Improve Customer
            Retention.
          </h2>
          <div class="d-flex gap-3">
            <a v-for="icon in socialIcon" :key="icon.id" :href="icon.link">
              <font-awesome-icon :icon="['fa-brands', icon.icon]" />
            </a>
          </div>
        </div>

        <div class="col-sm-2" v-for="element in footerLink" :key="element.id">
          <h6 class="pb-3">{{ element.title }}</h6>
          <ul>
            <li class="pb-3" v-for="(text, i) in element.text" :key="i">
              <a
                href="https://github.com/Ciro97cu"
                class="text-decoration-none"
              >
                {{ text }}
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import socialIcon from "../assets/data/socialIcon";
import footerLink from "../assets/data/footerLink";

export default {
  name: "FooterTop",
  data() {
    return {
      footerLink,
      socialIcon,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.col-sm-6 {
  h2 {
    max-width: 80%;
    font-weight: 600;
  }

  a {
    color: black;
    &:hover {
      color: $color-Ecstasy;
    }
  }
}

.col-sm-2 {
  h6 {
    font-weight: 600;
  }
  a {
    color: black;
    font-weight: 500;
    &:hover {
      color: $color-Ecstasy;
    }
  }
}
</style>