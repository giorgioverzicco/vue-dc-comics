<template>
  <p class="a-text">{{ text }}</p>
</template>

<script>
export default {
  name: "AText",
  props: {
    text: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.a-text {
  color: var(--clr-secondary-050);
}
</style>
