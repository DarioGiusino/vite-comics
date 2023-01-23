<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue'
import { headerLinks, comics } from './data/index.js'
export default {
  name: 'Comics Site',
  data() {
    return {
      headerLinks,
      comics
    }
  },
  components: { AppHeader, AppMain }
}
</script>

<template>
  <app-header :links="headerLinks"></app-header>
  <app-main></app-main>
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>