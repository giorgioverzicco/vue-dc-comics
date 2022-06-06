<template>
  <div class="a-badge">
    {{ content }}
  </div>
</template>

<script>
export default {
  name: "ABadge",
  props: {
    content: String,
  },
};
</script>

<style lang="scss" scoped>
.a-badge {
  padding: var(--spacing-3) var(--spacing-5);
  font-size: var(--fs-xl);
  font-weight: var(--fw-bold);
  color: var(--clr-secondary-050);
  background-color: var(--clr-primary-600);
  text-transform: uppercase;
}
</style>
