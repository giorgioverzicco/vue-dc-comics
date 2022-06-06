<template>
  <div class="o-footerContent">
    <div class="container">
      <OFooterSection v-for="(sect, idx) in sections" :key="sect.title + idx" :title="sect.title" :links="sect.links" />
      <img src="@/assets/img/dc-logo-bg.png" alt="" />
    </div>
  </div>
</template>

<script>
import OFooterSection from "./OFooterSection.vue";
export default {
  name: "OFooterContent",
  components: { OFooterSection },
  data() {
    return {
      sections: [
        {
          title: "DC Comics",
          links: [
            {
              title: "Characters",
              url: "#",
            },
            {
              title: "Comics",
              url: "#",
            },
            {
              title: "Movies",
              url: "#",
            },
            {
              title: "TV",
              url: "#",
            },
            {
              title: "Games",
              url: "#",
            },
            {
              title: "Collectibles",
              url: "#",
            },
            {
              title: "Videos",
              url: "#",
            },
            {
              title: "Fans",
              url: "#",
            },
            {
              title: "News",
              url: "#",
            },
          ],
        },
        {
          title: "Shop",
          links: [
            {
              title: "Shop DC",
              url: "#",
            },
            {
              title: "Shop DC Collectibles",
              url: "#",
            },
          ],
        },
        {
          title: "DC",
          links: [
            {
              title: "Terms Of Use",
              url: "#",
            },
            {
              title: "Privacy policy (New)",
              url: "#",
            },
            {
              title: "Advertising",
              url: "#",
            },
            {
              title: "Jobs",
              url: "#",
            },
            {
              title: "Subscriptions",
              url: "#",
            },
            {
              title: "Talent Workshops",
              url: "#",
            },
            {
              title: "CPSC Certificates",
              url: "#",
            },
            {
              title: "Ratings",
              url: "#",
            },
            {
              title: "Shop Help",
              url: "#",
            },
            {
              title: "Contact Us",
              url: "#",
            },
          ],
        },
        {
          title: "Sites",
          links: [
            {
              title: "DC",
              url: "#",
            },
            {
              title: "MAD Magazine",
              url: "#",
            },
            {
              title: "DC Kids",
              url: "#",
            },
            {
              title: "DC Universe",
              url: "#",
            },
            {
              title: "DC Power Visa",
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
.o-footerContent {
  position: relative;
  background-image: url("@/assets/img/footer-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  overflow: hidden;

  .container {
    display: flex;
    flex-wrap: wrap;
    gap: var(--spacing-8);
    padding-block: var(--spacing-6);
  }

  img {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%);
  }
}
</style>
