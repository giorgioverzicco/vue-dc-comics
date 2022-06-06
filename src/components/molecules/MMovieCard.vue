<template>
  <a class="m-movieCard" :href="url">
    <div class="m-movieCard__thumbnail" :style="{ backgroundImage: `url(${thumb})` }"></div>
    <span class="m-movieCard__title">{{ title }}</span>
  </a>
</template>

<script>
export default {
  name: "MMovieCard",
  props: {
    url: String,
    thumb: String,
    title: String,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.m-movieCard {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  gap: var(--spacing-3);
  width: 8rem;
  text-decoration: none;

  &__thumbnail {
    aspect-ratio: 1;
    width: 100%;
    background-color: red;
    background-repeat: no-repeat;
    background-size: cover;
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
