<template>
  <div class="o-footerTop">
    <div class="container">
      <MIconLink v-for="(link, idx) in links" :key="idx" :link="link" :icon="link.icon" />
    </div>
  </div>
</template>

<script>
import MIconLink from "../molecules/MIconLink.vue";
export default {
  components: { MIconLink },
  name: "OFooterTop",
  data() {
    return {
      links: [
        {
          name: "Digital Comics",
          url: "#",
          icon: {
            img: "buy-comics-digital-comics.png",
            alt: "icon",
          },
        },
        {
          name: "DC Merchandise",
          url: "#",
          icon: {
            img: "buy-comics-merchandise.png",
            alt: "icon",
          },
        },
        {
          name: "Subscription",
          url: "#",
          icon: {
            img: "buy-comics-subscriptions.png",
            alt: "icon",
          },
        },
        {
          name: "Comic Shop Locator",
          url: "#",
          icon: {
            img: "buy-comics-shop-locator.png",
            alt: "icon",
          },
        },
        {
          name: "DC Power Visa",
          url: "#",
          icon: {
            img: "buy-dc-power-visa.svg",
            alt: "icon",
          },
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-footerTop {
  color: var(--clr-secondary-050);
  background-color: var(--clr-primary-500);

  .container {
    @include flex(space-between);
    padding-block: var(--spacing-8);
  }
}
</style>
