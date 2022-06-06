<template>
  <section class="o-footerSection">
    <h3 class="o-footerSection__title">{{ title }}</h3>
    <ul class="o-footerSection__list">
      <MFooterSectionItem v-for="(link, idx) in links" :key="link.title + idx" :link="link" />
    </ul>
  </section>
</template>

<script>
import MFooterSectionItem from "../molecules/MFooterSectionItem.vue";

export default {
  name: "OFooterSection",
  components: { MFooterSectionItem },
  props: {
    title: String,
    links: Array,
  },
};
</script>

<style lang="scss" scoped>
.o-footerSection {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-4);
  z-index: 999;

  &__title {
    color: var(--clr-secondary-050);
    font-size: var(--fs-lg);
    font-weight: var(--fw-bold);
  }

  &__list {
    display: flex;
    flex-direction: column;
    gap: var(--spacing-2);
    list-style-type: none;
  }
}
</style>
