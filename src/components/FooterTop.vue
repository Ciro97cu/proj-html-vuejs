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
            <a href="https://it-it.facebook.com/">
              <font-awesome-icon icon="fa-brands fa-facebook-f" />
            </a>
            <a href="https://twitter.com/?lang=it">
              <font-awesome-icon icon="fa-brands fa-twitter" />
            </a>
            <a href="https://www.instagram.com/">
              <font-awesome-icon icon="fa-brands fa-instagram" />
            </a>
            <a href="https://www.youtube.com/">
              <font-awesome-icon icon="fa-brands fa-youtube" />
            </a>
            <a href="https://it.linkedin.com/">
              <font-awesome-icon icon="fa-brands fa-linkedin-in" />
            </a>
            <a
              href="https://www.tiktok.com/login?redirect_url=https%3A%2F%2Fwww.tiktok.com%2Fit-IT&lang=en&enter_method=mandatory"
            >
              <font-awesome-icon icon="fa-brands fa-tiktok" />
            </a>
          </div>
        </div>
        <div class="col-sm-2" v-for="(element, i) in footerLink" :key="i">
          <h6 class="pb-3">{{ element.title }}</h6>
          <ul>
            <li class="pb-3" v-for="(text, k) in element.text" :key="k">
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
import footerLink from "../assets/data/footerLink";

export default {
  name: "FooterTop",
  data() {
    return {
      footerLink,
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