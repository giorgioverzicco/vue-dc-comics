<template>
  <component class="a-title" :is="tag">
    {{ content }}
  </component>
</template>

<script>
export default {
  name: "ATitle",
  props: {
    tag: {
      type: String,
      required: true,
    },
    content: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.a-title {
  color: var(--clr-secondary-050);
}
</style>
