<template>
  <div>
    <div class="container-sm py-5">
      <div class="row align-items-center justify-content-around py-5">
        <div class="col-sm-5 text-wrapper d-flex flex-column gap-3">
          <h2>
            We Boost Our Client's Bottom Line by Optimizing Their Growth
            Potential.
          </h2>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Inventore
            molestias, est eaque exercitationem quasi eius debitis pariatur quis
            ut veritatis!
          </p>
          <button class="btn align-self-start">Why Work With Us</button>
        </div>
        <div class="col-sm-5">
          <img
            class="w-100"
            src="@/assets/img/we-boost-our-clients.jpg"
            alt="our-clients"
          />
        </div>
      </div>

      <div class="row align-items-center justify-content-around py-2">
        <div class="col-sm-5">
          <div class="d-flex flex-column">
            <div class="pb-5">
              <h3>We Build Relationships</h3>
              <p>
                Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus
                maximus nec ut leo. Integer consectetur.
              </p>
            </div>
            <div>
              <h3>Proprietary Processes</h3>
              <p>
                Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus
                maximus nec ut leo. Integer consectetur.
              </p>
            </div>
          </div>
        </div>
        <div class="col-sm-5">
          <div class="d-flex flex-column">
            <div class="pb-5 d-flex align-items-center">
              <div class="p-3 me-3 d-flex align-items-center border_orange">
                <font-awesome-icon
                  icon="fa-solid fa-magnifying-glass"
                  class="p-2 icon_bg_orange text-white rounded-3"
                />
              </div>
              <div class="d-flex flex-column">
                <h3 class="pb-2">Accountability</h3>
                <p>Curabitur ac leo nunc vestibulum</p>
              </div>
            </div>

            <div class="pb-5 d-flex align-items-center">
              <div class="p-3 me-3 d-flex align-items-center border_orange">
                <font-awesome-icon
                  icon="fa-solid fa-plus"
                  class="p-2 icon_bg_orange text-white rounded-3"
                />
              </div>
              <div class="d-flex flex-column">
                <h3 class="pb-2">Transparency</h3>
                <p>Curabitur ac leo nunc vestibulum</p>
              </div>
            </div>

            <div class="pb-5 d-flex align-items-center">
              <div class="p-3 me-3 d-flex align-items-center border_orange">
                <font-awesome-icon
                  icon="fa-solid fa-signal"
                  class="p-2 icon_bg_orange text-white rounded-3"
                />
              </div>
              <div class="d-flex flex-column">
                <h3 class="pb-2">Investment</h3>
                <p>Curabitur ac leo nunc vestibulum</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WorkWithus",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";
.col-sm-5 {
  h2 {
    font-size: 40px;
    font-weight: 700;
  }

  p {
    font-weight: 500;
  }

  button {
    @include button($color-Ecstasy, white, $color-Tango, black);
  }
}

.border_orange {
  border: 2px solid $color-Ecstasy;
  border-radius: 15px;
}

.icon_bg_orange {
  background-color: $color-Ecstasy;
}
</style>