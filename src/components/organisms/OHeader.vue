<template>
  <header class="o-header">
    <div class="container">
      <ALogo />
      <ONavbar :links="links" />
    </div>
  </header>
</template>

<script>
import ALogo from "../atoms/ALogo.vue";
import ONavbar from "./ONavbar.vue";

export default {
  name: "OHeader",
  components: { ALogo, ONavbar },
  data() {
    return {
      links: [
        {
          title: "Characters",
          url: "#",
          active: false,
        },
        {
          title: "Comics",
          url: "#",
          active: true,
        },
        {
          title: "Movies",
          url: "#",
          active: false,
        },
        {
          title: "TV",
          url: "#",
          active: false,
        },
        {
          title: "Games",
          url: "#",
          active: false,
        },
        {
          title: "Collectibles",
          url: "#",
          active: false,
        },
        {
          title: "Videos",
          url: "#",
          active: false,
        },
        {
          title: "Fans",
          url: "#",
          active: false,
        },
        {
          title: "News",
          url: "#",
          active: false,
        },
        {
          title: "Shop",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.o-header {
  background-color: #fff;

  .container {
    @include flex(space-between);
    gap: var(--spacing-4);
    padding-block: var(--spacing-4);
  }
}
</style>
