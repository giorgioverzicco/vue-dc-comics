<template>
  <footer class="o-footer">
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
  name: "OFooter",
  components: { OFooterTop, OFooterContent, OFooterBottom },
};
</script>
