<template>
  <footer>
    <OFooterTop />
    <MFooterContent />
    <MFooterBottom />
  </footer>
</template>

<script>
import MFooterBottom from "../molecules/MFooterBottom.vue";
import MFooterContent from "../molecules/MFooterContent.vue";
import OFooterTop from "./OFooterTop.vue";

export default {
  components: { OFooterTop, MFooterContent, MFooterBottom },
  name: "OFooter",
};
</script>

<style lang="scss" scoped></style>
