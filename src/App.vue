<template>
  <div id="app">
    <OHeader />
    <OMain />
    <OFooter />
  </div>
</template>

<script>
import OFooter from "./components/organisms/OFooter.vue";
import OHeader from "./components/organisms/OHeader.vue";
import OMain from "./components/organisms/OMain.vue";
export default {
  name: "App",
  components: { OHeader, OMain, OFooter },
};
</script>

<style lang="scss">
@import "@/assets/style/global";
</style>
