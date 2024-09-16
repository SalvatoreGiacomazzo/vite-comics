<script>
import AppHeader from './components/AppHeader.vue'
import AppFirstFooter from './components/AppFirstFooter.vue'
import AppSecondFooter from './components/AppSecondFooter.vue'
import AppContent from './components/AppContent.vue'
import AppIcons from './components/AppIcons.vue'
export default {
  components: {
    AppHeader,
    AppFirstFooter,
    AppSecondFooter,
    AppContent,
    AppIcons
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

  <!--Content-->
  <AppContent />

  <!--Stripe with Icons-->
  <AppIcons />
</template>

<style></style>
