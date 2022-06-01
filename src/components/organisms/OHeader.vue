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
header {
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-block: var(--spacing-5);
    background-color: #fff;
  }
}
</style>
