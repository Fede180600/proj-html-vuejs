<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- /HEADER -->

    <!-- MAIN -->
    <main>
      <!-- banner top -->
      <AppBannerTop />
      <!-- /banner top -->

      <!-- courses section -->
      <AppCoursesSection />
      <!-- /courses section -->

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
import AppCoursesSection from "./assets/components/AppCoursesSection"
export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppBannerTop,
    AppCoursesSection
  }
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
</style>
