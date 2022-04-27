<template>
  <div>
    <div class="offset-sm-2 col-sm-4 bg-white rounded-3 p-5">
      <div class="d-flex flex-column align-items-center gap-3">
        <div class="wrapper_img">
          <img
            class="rounded-circle w-100"
            src="@/assets/img/marketing-consultant-expert.jpg"
            alt="Richard Madsen"
          />
        </div>
        <h4>Richard Madsen</h4>
        <p>Marketing Consultant Expert</p>
        <div class="d-inline-block pe-3 telephone">
          <font-awesome-icon icon="fa-solid fa-phone" class="pe-2" />
          (555) 802-1234
        </div>
        <form class="w-100">
          <input
            class="d-block w-100 mb-3 p-2"
            type="text"
            placeholder="Your Name*"
          />
          <input
            class="d-block w-100 mb-3 p-2"
            type="email"
            placeholder="Your Email*"
          />
          <input
            class="d-block w-100 mb-3 p-2"
            type="tel"
            placeholder="Your Phone Number*"
          />
          <input
            class="d-block w-100 submit border-0 btn p-3"
            type="submit"
            value="Get a Callback"
          />
        </form>
        <p class="credits">By submitting my data I agree to be contacted</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MarketingExpertCard",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

.col-sm-4 {
  position: absolute;
  bottom: -10%;
  right: 0;
  box-shadow: 0px 10px 21px 10px rgba(0, 0, 0, 0.2);
  .wrapper_img {
    width: 100px;
  }
  h4 {
    font-weight: 500;
  }
  p {
    color: $color-Gunsmoke;
  }
  .telephone {
    color: $color-Ecstasy;
    font-weight: 500;
  }
  input {
    border: 2px solid $color-Gray-Nurse;
    border-radius: 5px;

    &[type="text"] {
      background: url(../assets/img/image.png) no-repeat;
      background-position: 95% 50%;
    }

    &::placeholder {
      color: $color-Tundora;
    }
  }

  .submit {
    @include button($color-Ecstasy, white, $color-Tango, black);
  }
  p:last-child {
    font-size: 12px;
    font-weight: 500;
  }
}
</style>