<template>
  <main class="o-main">
    <AHero />
    <div class="container">
      <ABadge content="Current Series" />
      <h1>Content goes here!</h1>
    </div>
  </main>
</template>

<script>
import ABadge from "../atoms/ABadge.vue";
import AHero from "../atoms/AHero.vue";

export default {
  name: "OMain",
  components: { AHero, ABadge },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-main {
  background-color: var(--clr-secondary-900);

  .container {
    position: relative;
    @include flex(flex-start);
    padding-block: var(--spacing-8);
  }

  h1 {
    font-size: var(--fs-2xl);
    font-weight: var(--fw-bold);
    color: var(--clr-secondary-050);
  }

  .a-badge {
    top: -25%;
    left: 0;
    transform: translateY(25%);
  }
}
</style>
