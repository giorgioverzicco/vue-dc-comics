<template>
  <main class="o-main">
    <div class="container">
      <h1>Content goes here!</h1>
    </div>
  </main>
</template>

<script>
export default {
  name: "OMain",
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-main {
  background-color: var(--clr-secondary-900);

  .container {
    @include flex(flex-start);
    padding-block: var(--spacing-8);
  }

  h1 {
    font-size: var(--fs-2xl);
    font-weight: var(--fw-bold);
    color: var(--clr-secondary-050);
  }
}
</style>
