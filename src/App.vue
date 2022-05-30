<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- /HEADER -->

    <!-- MAIN -->
    <main>
      <!-- app banner top -->
      <AppBannerTop />
      <!-- /app banner top -->
    </main>
    <!-- MAIN -->

    <!-- FOOTER -->
    <AppFooter />
    <!-- /FOOTER -->

  </div>
</template>

<script>
import AppHeader from "./assets/components/AppHeader.vue";
import AppFooter from "./assets/components/AppFooter.vue";
import AppBannerTop from "./assets/components/AppBannerTop.vue";
export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppBannerTop
  }
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";
</style>
