<template>
  <img class="a-icon" :src="require(`@/assets/img/${icon.img}`)" :alt="icon.alt" />
</template>

<script>
export default {
  name: "AIcon",
  props: {
    icon: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.a-icon {
  height: 100%;
}
</style>
