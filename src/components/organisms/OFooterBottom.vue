<template>
  <div class="o-footerBottom">
    <div class="container">
      <AButtonLink url="#" text="Sign-up now!" />
      <OFooterSocials />
    </div>
  </div>
</template>

<script>
import AButtonLink from "../atoms/AButtonLink.vue";
import OFooterSocials from "./OFooterSocials.vue";
export default {
  name: "OFooterBottom",
  components: { AButtonLink, OFooterSocials },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-footerBottom {
  color: var(--clr-secondary-050);
  background-color: var(--clr-secondary-800);

  .container {
    @include flex(space-between);
    padding-block: var(--spacing-6);
  }

  .a-buttonLink {
    text-transform: uppercase;
  }
}
</style>
