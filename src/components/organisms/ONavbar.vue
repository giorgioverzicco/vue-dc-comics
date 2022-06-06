<template>
  <nav class="o-navbar">
    <ul class="o-navbarList">
      <MNavbarItem v-for="(link, idx) in links" :key="link.title + idx" :link="link" />
    </ul>
  </nav>
</template>

<script>
import MNavbarItem from "../molecules/MNavbarItem.vue";
export default {
  name: "ONavbar",
  components: { MNavbarItem },
  props: {
    links: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-navbar {
  .o-navbarList {
    display: flex;
    flex-wrap: wrap;
    column-gap: var(--spacing-4);
    row-gap: var(--spacing-2);
    list-style-type: none;
  }
}
</style>
