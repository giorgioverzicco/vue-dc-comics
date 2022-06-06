<template>
  <a class="m-iconLink" :href="link.url">
    <AIcon :icon="icon" />
    <ALink :link="link" />
  </a>
</template>

<script>
import AIcon from "../atoms/AIcon.vue";
import ALink from "../atoms/ALink.vue";

export default {
  name: "MIconLink",
  components: { AIcon, ALink },
  props: {
    icon: Object,
    link: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.m-iconLink {
  @include flex(flex-start);
  gap: var(--spacing-2);
  color: inherit;
  text-decoration: none;
}
</style>
