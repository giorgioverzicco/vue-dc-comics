<template>
  <a class="m-iconLink" :href="link.url">
    <AIcon :icon="icon" />
    <AText :text="link.name" />
  </a>
</template>

<script>
import AIcon from "../atoms/AIcon.vue";
import AText from "../atoms/AText.vue";

export default {
  components: { AIcon, AText },
  props: {
    link: {
      type: Object,
      required: true,
    },
    icon: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.m-iconLink {
  @include flex(flex-start);
  text-decoration: none;
  text-transform: uppercase;

  .a-text {
    margin-left: var(--spacing-4);
  }

  .a-icon {
    height: 3.5rem;
  }

  &:last-of-type .a-icon {
    height: 2.5rem;
  }
}
</style>
