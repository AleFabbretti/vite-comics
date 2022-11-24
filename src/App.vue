<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppDcBar from './components/AppDcBar.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppDcBar,
    AppFooter
  }
}
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppDcBar/>
  <AppFooter/>
</template>

<style lang="scss">
@import './style/global.scss';
</style>
