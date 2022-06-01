<template>
  <section class="m-linkList">
    <ATitle tag="h3" :content="title" />
    <ul class="m-linkList__list">
      <li class="m-linkList__item" v-for="(link, idx) in links" :key="idx">
        <ALink :link="link" />
      </li>
    </ul>
  </section>
</template>

<script>
import ALink from "../atoms/ALink.vue";
import ATitle from "../atoms/ATitle.vue";

export default {
  components: { ATitle, ALink },
  props: {
    title: {
      type: String,
      required: true,
    },
    links: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.m-linkList {
  .a-title {
    text-transform: uppercase;
    font-size: var(--fs-xl);
    letter-spacing: var(--ls-sm);
    margin-bottom: var(--spacing-3);
  }

  .a-link {
    font-size: var(--fs-sm);
    color: var(--clr-secondary-500);
  }

  &__list {
    display: flex;
    flex-direction: column;
    row-gap: var(--spacing-1);
    list-style-type: none;
  }
}
</style>
