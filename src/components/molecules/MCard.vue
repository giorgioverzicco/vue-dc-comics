<template>
  <a class="m-card" :href="url">
    <img class="m-card__thumbnail" :src="thumb" alt="" />
    <span class="m-card__title">{{ title }}</span>
  </a>
</template>

<script>
export default {
  name: "MCard",
  props: {
    url: String,
    thumb: String,
    title: String,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.m-card {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  gap: var(--spacing-3);
  width: 10rem;
  text-decoration: none;

  &__thumbnail {
    aspect-ratio: 1;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }

  &__title {
    font-size: var(--fs-xs);
    font-weight: var(--fw-normal);
    color: var(--clr-secondary-050);
    text-transform: uppercase;
    word-break: break-all;
  }
}
</style>
