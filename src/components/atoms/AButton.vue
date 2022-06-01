<template>
  <button class="button">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "AButton",
  props: {
    text: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.button {
  padding: var(--spacing-3) var(--spacing-4);
  font-size: var(--fs-md);
  font-weight: var(--fw-normal);
  color: var(--clr-secondary-050);
  background-color: transparent;
  border: none;
  cursor: pointer;

  &.-primary {
    font-size: var(--fs-lg);
    border: 0.125rem solid var(--clr-primary-500);
  }

  &.-uppercase {
    text-transform: uppercase;
  }
}
</style>
