<template>
  <a class="a-buttonLink" :href="url">{{ text }}</a>
</template>

<script>
export default {
  name: "AButtonLink",
  props: {
    url: String,
    text: String,
  },
};
</script>

<style lang="scss" scoped>
.a-buttonLink {
  font-size: var(--fs-md);
  font-weight: var(--fw-bold);
  padding: var(--spacing-3) var(--spacing-4);
  color: inherit;
  background-color: transparent;
  border: 0.125rem solid var(--clr-primary-500);
  text-decoration: none;
}
</style>
