<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader :headerNavItems="headerVoices"/>
    <!-- /HEADER -->

    <!-- MAIN -->
    <main>
      <!-- banner top -->
      <AppBannerTop />
      <!-- /banner top -->

      <!-- courses section -->
      <AppCoursesSection />
      <!-- /courses section -->

      <!-- my book jumbotron -->
      <AppBookJumbotron />
      <!-- /my book jumbotron  -->

      <!-- why my courses section -->
      <AppWhySection />
      <!-- /why my courses section -->

      <!-- app statistcs jumbtron  -->
      <AppStatisticsJumbotron />
      <!-- /app statistcs jumbtron  -->

      <!-- app prefooter section -->
      <AppPrefooterSection />
      <!-- app prefooter section -->

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
import AppCoursesSection from "./assets/components/AppCoursesSection.vue";
import AppBookJumbotron from "./assets/components/AppBookJumbotron.vue";
import AppWhySection from "./assets/components/AppWhySection.vue";
import AppStatisticsJumbotron from "./assets/components/AppStatisticsJumbotron.vue";
import AppPrefooterSection from "./assets/components/AppPrefooterSection.vue"

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppBannerTop,
    AppCoursesSection,
    AppBookJumbotron,
    AppWhySection,
    AppStatisticsJumbotron,
    AppPrefooterSection
  },
  data() {
    return {
      headerVoices: [
      {
        content: 'Courses',
        id: 1
      },
      {
        content: 'Courses Formats',
        id: 2
      },
      {
        content: 'Add Course',
        id: 3
      },
      {
        content: 'Pages',
        id: 4
      },
      {
        content: 'Demos',
        id: 5
      }
      ]
    }
  },
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
</style>
