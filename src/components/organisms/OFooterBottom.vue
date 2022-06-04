<template>
  <div class="o-footerBottom">
    <div class="container">
      <AButton class="-primary -uppercase" text="Sign-up now!" />
      <MSocials />
    </div>
  </div>
</template>

<script>
import AButton from "../atoms/AButton.vue";
import MSocials from "../molecules/MSocials.vue";
export default {
  components: { AButton, MSocials },
  name: "OFooterBottom",
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-footerBottom {
  color: var(--clr-secondary-050);
  background-color: var(--clr-secondary-800);

  .container {
    @include flex(space-between);
    flex-wrap: wrap;
    row-gap: var(--spacing-4);
    padding-block: var(--spacing-6);
  }
}
</style>
