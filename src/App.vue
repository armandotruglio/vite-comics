<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppNav from "./components/AppNav.vue"

export default {
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppNav
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppNav />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
