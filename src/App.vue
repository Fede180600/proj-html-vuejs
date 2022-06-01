<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader :headerNavItems="headerVoices"/>
    <!-- /HEADER -->

    <!-- MAIN -->
    <main>
      <!-- banner top -->
      <AppBannerTop :countdown="countdownElements"/>
      <!-- /banner top -->

      <!-- courses section -->
      <AppCoursesSection :coursesArray="courses"/>
      <!-- /courses section -->

      <!-- my book jumbotron -->
      <AppBookJumbotron />
      <!-- /my book jumbotron  -->

      <!-- why my courses section -->
      <AppWhySection :whyArray="why"/>
      <!-- /why my courses section -->

      <!-- app statistcs jumbtron  -->
      <AppStatisticsJumbotron :statisticsArray="statistics"/>
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
          id: 1,
          new: null
          
        },
        {
          content: 'Courses Formats',
          id: 2,
          new: null
        },
        {
          content: 'Add Course',
          id: 3,
          new: true
        },
        {
          content: 'Pages',
          id: 4,
          new: null
        },
        {
          content: 'Demos',
          id: 5,
          new: null
        }
      ],
      countdownElements: [
        {
          number: 26,
          description: "Days"
        },
        {
          number: 12,
          description: "Hours"
        },
        {
          number: 47,
          description: "Minutes"
        },
        {
          number: 34,
          description: "Seconds"
        },
      ],
      courses: [
        {
          poster: "photo-1496307042754-b4aa456c4a2d-370x200.jpeg",
          title: "How to be a DJ? Make Elettronic Music",
          type: "Electronic",
          level: "Advanced",
          lectures: "8 Lectures",
          duration: "6 Hours",
          special: true
        },
        {
          poster: "12345-1-370x200.png",
          title: "Nvidia and UE4 Technologies Practice",
          type: "Nvidia",
          level: "Advanced",
          lectures: "8 Lectures",
          duration: "6 Hours",
          special: true
        },
        {
          poster: "photo-1491897554428-130a60dd4757-370x200.jpeg",
          title: "Fashion Photography from professional",
          type: "Fashion",
          level: "Advanced",
          lectures: "6 Lectures",
          duration: "6 Hours",
          special: true
        },
        {
          poster: "photo-1416339134316-0e91dc9ded92-370x200.jpeg",
          title: "Design Instruments for Communication",
          type: "Comunication",
          level: "Intermediate",
          lectures: "6 Lectures",
          duration: "6 Hours",
          special: null
        },
        {
          poster: "cathryn-lavery-67852-unsplash-370x200.jpg",
          title: "Make your Concept Right and Beautiful",
          type: "Art",
          level: "Intermediate",
          lectures: "6 Lectures",
          duration: "6 Hours",
          special: null
        },
        {
          poster: "photo-1475452779376-caebfb988090-370x200.jpeg",
          title: "Road Bike Manual or How to Be a Champion.",
          type: "Bicycling",
          level: "Advanced",
          lectures: "6 Lectures",
          duration: "6 Hours",
          special: null
        }
      ],
      why: [
        {
          icon: "fas fa-briefcase",
          title: "Entrepreneurship",
          text: "Vestibulum vitae aliquam nunc. Suspendisse mollis metus ac tellus egestas pharetra. Suspendisse at     viverra purus. Pellentesque nec posuere ligula, eu congue leo. Integer vulputate tempor arcu. Vestibulum vulputate"
        },
        {
          icon: "fas fa-rocket",
          title: "Accelerated learning",
          text: "Vestibulum vitae aliquam nunc. Suspendisse mollis metus ac tellus egestas pharetra. Suspendisse at     viverra purus. Pellentesque nec posuere ligula, eu congue leo. Integer vulputate tempor arcu. Vestibulum vulputate"
        },
        {
          icon: "fas fa-thumbs-up",
          title: "Productivity",
          text: "Vestibulum vitae aliquam nunc. Suspendisse mollis metus ac tellus egestas pharetra. Suspendisse at     viverra purus. Pellentesque nec posuere ligula, eu congue leo. Integer vulputate tempor arcu. Vestibulum vulputate"
        },
        {
          icon: "fas fa-cog",
          title: "Life Coaching",
          text: "Vestibulum vitae aliquam nunc. Suspendisse mollis metus ac tellus egestas pharetra. Suspendisse at     viverra purus. Pellentesque nec posuere ligula, eu congue leo. Integer vulputate tempor arcu. Vestibulum vulputate"
        },
        
      ],
      statistics: [
        {
          icon: "fas fa-user-friends",
          number: 3195,
          text: "Online Learner"
        },
        {
          icon: "fas fa-film",
          number: 23,
          text: "Video Corses"
        },
        {
          icon: "fas fa-image",
          number: 437,
          text: "Sliders & Images"
        },
        {
          icon: "fas fa-thumbs-up",
          number: 1440,
          text: "Excellent Reviews"
        },
      ]
    }
  },
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
</style>
