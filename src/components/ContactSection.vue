<template>
  <div id="contact_container">
    <div class="container-sm py-5">
      <div class="row py-5">
        <div class="col-sm-6 text-white">
          <h1 class="pb-4">Let's Make Things Happen</h1>
          <p class="pb-4">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet
            error blanditiis nostrum culpa veritatis nihil officiis incidunt rem
            impedit quos.
          </p>
          <div class="line my-4"></div>
          <p class="pb-4">
            <em
              >"The team at Avda Marketing Consultant is fabulous. They helped
              us unlock our potential online and offline. We have experienced
              year on year growth due to their progressive approach."
            </em>
          </p>
          <h5 class="pb-2">George Anderson</h5>
          <p>Digitalbox CEO</p>
        </div>
        <MarketingExpertCard id="card_contact" />
      </div>
    </div>
  </div>
</template>

<script>
import MarketingExpertCard from "./MarketingExpertCard.vue";

export default {
  name: "ContactSection",
  components: {
    MarketingExpertCard,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

#contact_container {
  padding: 50px 0;
  background-color: black;

  .row {
    position: relative;

    .col-sm-6 > * {
      max-width: 80%;
    }

    h1 {
      font-size: 50px;
      font-weight: 700;
    }

    .line {
      width: 80px;
      height: 1px;
      background-color: white;
    }

    #card_contact {
      box-shadow: none;
      position: absolute;
      top: 105%;
    }
  }
}
</style>