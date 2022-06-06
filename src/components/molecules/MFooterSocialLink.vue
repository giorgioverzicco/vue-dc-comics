<template>
  <a class="m-footerSocialLink" :href="social.url">
    <AIcon :icon="social.icon" />
  </a>
</template>

<script>
import AIcon from "../atoms/AIcon.vue";
export default {
  name: "MFooterSocialLink",
  components: { AIcon },
  props: {
    social: Object,
  },
};
</script>

<style lang="scss" scoped>
.m-footerSocialLink {
  color: inherit;
  text-decoration: none;

  .a-icon {
    width: 2rem;
    height: 2rem;
  }
}
</style>
