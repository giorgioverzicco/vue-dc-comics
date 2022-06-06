<template>
  <li class="m-navbarItem" :class="{ '-active': link.active }">
    <ALink :link="link" />
  </li>
</template>

<script>
import ALink from "../atoms/ALink.vue";

export default {
  name: "MNavbarItem",
  components: { ALink },
  props: {
    link: Object,
  },
};
</script>

<style lang="scss" scoped>
.m-navbarItem {
  position: relative;
  font-size: var(--fs-sm);
  font-weight: var(--fw-bold);
  color: var(--clr-secondary-700);
  text-transform: uppercase;

  &:hover,
  &:focus,
  &.-active {
    color: var(--clr-primary-500);
  }

  &.-active {
    border-bottom: 0.375rem solid var(--clr-primary-500);
    margin-bottom: -3.7rem;
  }
}
</style>
