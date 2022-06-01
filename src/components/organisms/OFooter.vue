<template>
  <footer>
    <OFooterTop />
    <OFooterContent />
    <OFooterBottom />
  </footer>
</template>

<script>
import OFooterBottom from "./OFooterBottom.vue";
import OFooterContent from "./OFooterContent.vue";
import OFooterTop from "./OFooterTop.vue";

export default {
  components: { OFooterTop, OFooterContent, OFooterBottom },
  name: "OFooter",
};
</script>

<style lang="scss" scoped></style>
