<script>
import AppHeader from './components/AppHeader.vue'
import AppFirstFooter from './components/AppFirstFooter.vue'
import AppSecondFooter from './components/AppSecondFooter.vue'
import AppContent from './components/AppContent.vue'
import AppIcons from './components/AppIcons.vue'
import AppJumbotron from './components/AppJumbotron.vue'

export default {
  components: {
    AppHeader,
    AppFirstFooter,
    AppSecondFooter,
    AppContent,
    AppIcons,
    AppJumbotron,
  
  },
  data() {
    return {

    }
  }
}
</script>

<template>

  <!--Header-->
  <AppHeader />
<!--Jumbotron-->
<AppJumbotron />
  <!--Content-->
  <AppContent />
  <!--Stripe with Icons-->
  <AppIcons />
  <!--First Footer-->
  <AppFirstFooter />
  <!--Second footer-->
  <AppSecondFooter />
</template>

<style></style>
