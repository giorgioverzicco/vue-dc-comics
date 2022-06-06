<template>
  <div class="a-icon">
    <img :src="require(`@/assets/${icon.src}`)" :alt="icon.alt" />
  </div>
</template>

<script>
export default {
  name: "AIcon",
  props: {
    icon: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/mixins";

.a-icon {
  @include flex;
  width: 4rem;
  height: 4rem;

  img {
    max-width: 100%;
    height: 100%;
  }
}
</style>
