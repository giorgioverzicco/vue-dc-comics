<template>
  <div class="o-stores">
    <div class="container">
      <MIconLink v-for="(link, idx) in links" :key="link.title + idx" :icon="link.icon" :link="link" />
    </div>
  </div>
</template>

<script>
import MIconLink from "../molecules/MIconLink.vue";
export default {
  name: "OFooterTop",
  components: { MIconLink },
  data() {
    return {
      links: [
        {
          title: "Digital Comics",
          url: "#",
          icon: {
            src: "img/buy-comics-digital-comics.png",
            alt: "icon",
          },
        },
        {
          title: "DC Merchandise",
          url: "#",
          icon: {
            src: "img/buy-comics-merchandise.png",
            alt: "icon",
          },
        },
        {
          title: "Subscription",
          url: "#",
          icon: {
            src: "img/buy-comics-subscriptions.png",
            alt: "icon",
          },
        },
        {
          title: "Comic Shop Locator",
          url: "#",
          icon: {
            src: "img/buy-comics-shop-locator.png",
            alt: "icon",
          },
        },
        {
          title: "DC Power Visa",
          url: "#",
          icon: {
            src: "img/buy-dc-power-visa.svg",
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

.o-stores {
  color: var(--clr-secondary-050);
  background-color: var(--clr-primary-500);

  .container {
    @include flex(space-between);
    flex-wrap: wrap;
    row-gap: var(--spacing-4);
    padding-block: var(--spacing-8);
  }

  .m-iconLink {
    text-transform: uppercase;
  }
}
</style>
