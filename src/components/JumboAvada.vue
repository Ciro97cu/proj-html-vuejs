<template>
  <div id="jumbo" class="py-3">
    <div class="container-sm">
      <div class="row align-items-center justify-content-between">
        <div class="col-sm-6 text-white">
          <h1 class="pb-4">Unlock Your Online Growth Potential</h1>
          <p class="pb-4">
            Online Marketing to secure customer retention, leads, and sales. We
            focus on the bigger picture.
          </p>
          <button class="btn border border-white">
            Our Services
            <font-awesome-icon icon="fa-solid fa-arrow-right" class="ps-2" />
          </button>
        </div>
        <div class="offset-sm-2 col-sm-4 bg-white rounded-3 p-4">
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
    </div>
  </div>
</template>

<script>
export default {
  name: "JumboAvada",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
@import "../assets/style/mixin.scss";

#jumbo {
  background-image: url(../assets/img/marketing-intro.jpg);
  background-size: cover;

  .row {
    min-height: 700px;

    .col-sm-6 {
      h1 {
        font-size: 50px;
        font-weight: 700;
      }

      p {
        font-size: 25px;
      }

      button {
        @include button(white, black, transparent, white);
      }
    }

    .col-sm-4 {
      .wrapper_img {
        width: 70px;
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
        &::placeholder {
          color: $color-Tundora;
        }
      }

      .submit {
        @include button($color-Ecstasy, white, $color-Ecstasy-Op, black);
      }
      p:last-child {
        font-size: 12px;
        font-weight: 500;
      }
    }
  }
}
</style>