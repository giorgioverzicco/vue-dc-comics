<template>
  <button class="a-button">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "AButton",
  props: {
    text: String,
  },
};
</script>

<style lang="scss" scoped>
.a-button {
  padding: var(--spacing-3) var(--spacing-5);
  font-size: var(--fs-sm);
  color: inherit;
  background-color: transparent;
  border: none;
  cursor: pointer;

  &.-primary {
    font-weight: var(--fw-bold);
    color: var(--clr-secondary-050);
    background-color: var(--clr-primary-600);
  }

  &.-large {
    padding-inline: var(--spacing-8);
  }

  &.-uppercase {
    text-transform: uppercase;
  }
}
</style>
