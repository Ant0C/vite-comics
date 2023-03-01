<script>
import AppHeader from './components/AppMain.vue'
import AppMain from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <div>
    <AppMain></AppMain>
    <AppHeader></AppHeader>
    <AppFooter></AppFooter>
  </div>
</template>

<style>
@use './style/general.scss';
</style>
