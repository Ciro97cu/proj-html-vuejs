<template>
  <div>
    <div class="container-sm pb-5">
      <div class="row align-items-center pb-5">
        <div class="col-sm-6">
          <em
            >&copy; 2020 <span class="mini_bullet">•</span> Avada Consultant
            <span class="mini_bullet">•</span> Powered by WordPress</em
          >
        </div>
        <div class="col-sm-3">
          <em>Call Us (555) 802-1234</em>
        </div>
        <div class="col-sm-3 text-end">
          <em>info@yourcompany.com</em>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBottom",
};
</script>

<style lang="scss" scoped>
em {
  font-size: 14px;

  .mini_bullet {
    font-size: 20px;
  }
}
</style>