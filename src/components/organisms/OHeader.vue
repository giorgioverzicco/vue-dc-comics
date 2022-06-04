<template>
  <header>
    <div class="container">
      <ALogo />
      <MNavbar :links="links" />
    </div>
  </header>
</template>

<script>
import ALogo from "../atoms/ALogo.vue";
import MNavbar from "../molecules/MNavbar.vue";

export default {
  name: "OHeader",
  components: { MNavbar, ALogo },
  data() {
    return {
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
        {
          name: "Shop",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

header {
  background-color: #fff;

  .container {
    @include flex(space-between);
    gap: var(--spacing-4);
    padding-block: var(--spacing-5);
  }
}
</style>
