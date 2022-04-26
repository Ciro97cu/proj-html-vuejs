<template>
  <div>
    <div class="container-sm py-5">
      <div class="row align-items-center justify-content-around py-5">
        <div class="col-sm-5">
          <img class="w-100" src="@/assets/img/svg/img1.svg" alt="img1" />
        </div>
        <div class="col-sm-5 text-wrapper d-flex flex-column gap-3">
          <h6>
            <font-awesome-icon
              icon="fa-solid fa-circle-check"
              class="fa_blue"
            />
            Business Growth
          </h6>
          <h2>Invrease Brand Awareness</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea dicta
            mollitia eos fuga saepe unde vel dolorem maiores, quidem enim
            nesciunt earum quibusdam.
          </p>
          <button class="btn align-self-start">Get a Consultation</button>
        </div>
      </div>

      <div class="row align-items-center justify-content-around py-5">
        <div class="col-sm-5 text-wrapper d-flex flex-column gap-3">
          <h6>
            <font-awesome-icon
              icon="fa-solid fa-circle-check"
              class="fa_yellow"
            />
            Investors In People
          </h6>
          <h2>In-House Sales Training</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea dicta
            mollitia eos fuga saepe unde vel dolorem maiores, quidem enim
            nesciunt earum quibusdam.
          </p>
          <button class="btn align-self-start">Get a Consultation</button>
        </div>
        <div class="col-sm-5">
          <img class="w-100" src="@/assets/img/svg/img2.svg" alt="img2" />
        </div>
      </div>

      <div class="row align-items-center justify-content-around py-5">
        <div class="col-sm-5">
          <img class="w-100" src="@/assets/img/svg/img3.svg" alt="img3" />
        </div>
        <div class="col-sm-5 text-wrapper d-flex flex-column gap-3">
          <h6>
            <font-awesome-icon
              icon="fa-solid fa-circle-check"
              class="fa_green"
            />
            Social Media Analysis
          </h6>
          <h2>Harness Your Social Proof</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea dicta
            mollitia eos fuga saepe unde vel dolorem maiores, quidem enim
            nesciunt earum quibusdam.
          </p>
          <button class="btn align-self-start">Get a Consultation</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GeneralInfo",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

.text-wrapper {
  width: 400px;

  h2 {
    font-size: 50px;
  }

  p {
    font-size: 20px;
    font-weight: 500;
  }

  button {
    @include button($color-Ecstasy, white, $color-Tango, black);
  }

  .fa_blue {
    color: $color-Cerulean-Blue;
  }

  .fa_yellow {
    color: $color-Golden-Dream;
  }

  .fa_green {
    color: $color-Puerto-Rico;
  }
}
</style>