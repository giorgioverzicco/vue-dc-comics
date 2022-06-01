<template>
  <div class="m-socials">
    <AText text="Follow us" />
    <AIcon v-for="(icon, idx) in icons" :key="idx" :icon="icon" />
  </div>
</template>

<script>
import AIcon from "../atoms/AIcon.vue";
import AText from "../atoms/AText.vue";
export default {
  components: { AText, AIcon },
  data() {
    return {
      icons: [
        {
          img: "footer-facebook.png",
          alt: "Facebook",
        },
        {
          img: "footer-twitter.png",
          alt: "Twitter",
        },
        {
          img: "footer-youtube.png",
          alt: "YouTube",
        },
        {
          img: "footer-pinterest.png",
          alt: "Pinteres",
        },
        {
          img: "footer-periscope.png",
          alt: "Periscope",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.m-socials {
  @include flex();
  gap: var(--spacing-4);

  .a-text {
    font-size: var(--fs-xl);
    font-weight: var(--fw-bold);
    color: var(--clr-primary-500);
    text-transform: uppercase;
    margin-right: var(--spacing-2);
  }
}
</style>
