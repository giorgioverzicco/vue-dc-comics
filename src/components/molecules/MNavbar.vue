<template>
  <nav class="m-navbar">
    <ul class="m-navbar__menu">
      <li class="m-navbar__item" v-for="(link, idx) in links" :key="idx">
        <ALink :link="link" />
      </li>
    </ul>
  </nav>
</template>

<script>
import ALink from "../atoms/ALink.vue";

export default {
  components: { ALink },
  name: "MNavbar",
  props: {
    links: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.m-navbar {
  &__menu {
    display: flex;
    column-gap: var(--spacing-6);
    font-size: var(--fs-sm);
    font-weight: var(--fw-bold);
    letter-spacing: var(--ls-sm);
    text-transform: uppercase;
    list-style-type: none;
  }

  &__item {
    &:hover > * {
      color: var(--clr-primary-400);
    }
  }
}
</style>
