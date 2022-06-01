<template>
  <div class="o-footerContent">
    <div class="container">
      <MLinkList v-for="(section, idx) in sections" :key="idx" :title="section.title" :links="section.links" />
      <img src="@/assets/img/dc-logo-bg.png" alt="" />
    </div>
  </div>
</template>

<script>
import MLinkList from "../molecules/MLinkList.vue";
export default {
  components: { MLinkList },
  name: "OFooterContent",
  data() {
    return {
      sections: [
        {
          title: "DC Comics",
          links: [
            {
              name: "Characters",
              url: "#",
            },
            {
              name: "Comics",
              url: "#",
            },
            {
              name: "Movies",
              url: "#",
            },
            {
              name: "TV",
              url: "#",
            },
            {
              name: "Games",
              url: "#",
            },
            {
              name: "Collectibles",
              url: "#",
            },
            {
              name: "Videos",
              url: "#",
            },
            {
              name: "Fans",
              url: "#",
            },
            {
              name: "News",
              url: "#",
            },
          ],
        },
        {
          title: "Shop",
          links: [
            {
              name: "Shop DC",
              url: "#",
            },
            {
              name: "Shop DC Collectibles",
              url: "#",
            },
          ],
        },
        {
          title: "DC",
          links: [
            {
              name: "Terms Of Use",
              url: "#",
            },
            {
              name: "Privacy policy (New)",
              url: "#",
            },
            {
              name: "Advertising",
              url: "#",
            },
            {
              name: "Jobs",
              url: "#",
            },
            {
              name: "Subscriptions",
              url: "#",
            },
            {
              name: "Talent Workshops",
              url: "#",
            },
            {
              name: "CPSC Certificates",
              url: "#",
            },
            {
              name: "Ratings",
              url: "#",
            },
            {
              name: "Shop Help",
              url: "#",
            },
            {
              name: "Contact Us",
              url: "#",
            },
          ],
        },
        {
          title: "Sites",
          links: [
            {
              name: "DC",
              url: "#",
            },
            {
              name: "MAD Magazine",
              url: "#",
            },
            {
              name: "DC Kids",
              url: "#",
            },
            {
              name: "DC Universe",
              url: "#",
            },
            {
              name: "DC Power Visa",
              url: "#",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-footerContent {
  position: relative;
  color: var(--clr-secondary-050);
  background-color: var(--clr-primary-900);
  background-image: url("@/assets/img/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;

  .container {
    @include flex(flex-start, flex-start);
    flex-direction: column wrap;
    gap: var(--spacing-5);
    padding-block: var(--spacing-7);
  }

  img {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%);
  }
}
</style>
