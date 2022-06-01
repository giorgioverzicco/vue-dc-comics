<template>
  <a class="a-link" :href="link.url">{{ link.name }}</a>
</template>

<script>
export default {
  name: "ALink",
  props: {
    link: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.a-link {
  display: inline-block;
  color: var(--clr-secondary-600);
  text-decoration: none;
}
</style>
