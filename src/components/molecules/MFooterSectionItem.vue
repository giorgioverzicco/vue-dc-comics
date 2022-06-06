<template>
  <li class="m-footerSectionItem">
    <ALink :link="link" />
  </li>
</template>

<script>
import ALink from "../atoms/ALink.vue";
export default {
  name: "MFooterSectionItem",
  components: { ALink },
  props: {
    link: Object,
  },
};
</script>

<style lang="scss" scoped>
.m-footerSectionItem {
  color: var(--clr-secondary-500);
  font-size: var(--fs-sm);
  font-weight: var(--fw-normal);
}
</style>
