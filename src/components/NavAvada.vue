<template>
  <div>
    <div class="container-sm py-3">
      <div class="row align-items-center justify-content-between">
        <div class="col-auto">
          <div class="wrapper_img">
            <img
              class="w-100"
              src="@/assets/img/avada-marketing-logo-2x-400x74.png"
              alt="avada-marketing-logo"
            />
          </div>
        </div>
        <div class="col-auto">
          <ul>
            <li
              class="d-inline-block mx-3 pb-1"
              v-for="item in navLink"
              :key="item.name"
            >
              {{ item.name }}
              <font-awesome-icon
                v-if="item.dropdown"
                icon="fa-solid fa-chevron-down"
              />
            </li>
          </ul>
        </div>
        <div class="col-auto">
          <div class="d-inline-block pe-3">
            <font-awesome-icon icon="fa-solid fa-phone" class="pe-2" />
            (555) 802-1234
          </div>
          <button class="btn">Free Quote</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import navLink from "@/assets/data/navLink";

export default {
  name: "NavAvada",
  data() {
    return {
      navLink,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";
.wrapper_img {
  width: 150px;
}

.col-auto {
  font-size: 12px;
  font-weight: 700;
}

.fa-chevron-down {
  font-size: 10px;
}

.fa-phone {
  color: $color-Ecstasy;
}

li {
  font-size: 12px;
  @include navHover($color-Ecstasy);
}

button {
  @include button($color-Ecstasy-Op, $color-Ecstasy, $color-Ecstasy, white);
}
</style>