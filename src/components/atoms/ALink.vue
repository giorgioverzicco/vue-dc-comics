<template>
  <a class="a-link" :href="link.url">{{ link.title }}</a>
</template>

<script>
export default {
  name: "ALink",
  props: {
    link: Object,
  },
};
</script>

<style lang="scss" scoped>
.a-link {
  color: inherit;
  text-decoration: none;
}
</style>
