<template>
  <div class="o-footerSocials">
    <span class="o-footerSocials__title">Follow us</span>
    <MFooterSocialLink v-for="(social, idx) in socials" :key="social.icon.alt + idx" :social="social" />
  </div>
</template>

<script>
import MFooterSocialLink from "../molecules/MFooterSocialLink.vue";
export default {
  name: "MFooterSocial",
  components: { MFooterSocialLink },
  data() {
    return {
      socials: [
        {
          url: "#",
          icon: {
            src: "img/footer-facebook.png",
            alt: "Facebook",
          },
        },
        {
          url: "#",
          icon: {
            src: "img/footer-twitter.png",
            alt: "Twitter",
          },
        },
        {
          url: "#",
          icon: {
            src: "img/footer-youtube.png",
            alt: "YouTube",
          },
        },
        {
          url: "#",
          icon: {
            src: "img/footer-pinterest.png",
            alt: "Pinterest",
          },
        },
        {
          url: "#",
          icon: {
            src: "img/footer-periscope.png",
            alt: "Periscope",
          },
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-footerSocials {
  @include flex(flex-start);
  gap: var(--spacing-4);

  &__title {
    font-size: var(--fs-xl);
    font-weight: var(--fw-bold);
    color: var(--clr-primary-600);
    margin-right: var(--spacing-2);
    text-transform: uppercase;
  }
}
</style>
