<template>
  <main class="o-main">
    <AHero />
    <div class="container">
      <ABadge content="Current Series" />
      <OCurrentSeries />
    </div>
  </main>
</template>

<script>
import ABadge from "../atoms/ABadge.vue";
import AHero from "../atoms/AHero.vue";
import OCurrentSeries from "./OCurrentSeries.vue";

export default {
  name: "OMain",
  components: { AHero, OCurrentSeries, ABadge },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-main {
  background-color: var(--clr-secondary-900);

  .container {
    position: relative;
    @include flex(flex-start);
    padding-top: var(--spacing-7);
    padding-bottom: var(--spacing-4);
  }

  h1 {
    font-size: var(--fs-2xl);
    font-weight: var(--fw-bold);
    color: var(--clr-secondary-050);
  }

  .a-badge {
    position: absolute;
    top: -1.5rem;
    left: 0;
  }
}
</style>
