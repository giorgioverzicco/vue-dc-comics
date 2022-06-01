<template>
  <main>
    <div class="container">
      <h1>Content goes here</h1>
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

main {
  color: var(--clr-secondary-050);
  background-color: var(--clr-secondary-900);

  .container {
    @include flex(flex-start);
    padding-block: var(--spacing-8);
  }
}
</style>
