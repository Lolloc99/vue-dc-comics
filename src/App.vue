<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppFooter />
    <AppFooterBottom />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppFooterBottom from "./components/AppFooterBottom.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppFooterBottom,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
