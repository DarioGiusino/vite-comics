<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppNav from './components/AppNav.vue';
import { headerLinks, comics } from './data/index.js';
export default {
  name: 'Comics Site',
  data() {
    return {
      headerLinks,
      comics
    }
  },
  components: { AppHeader, AppMain, AppNav }
}
</script>

<template>
  <app-header :links="headerLinks"></app-header>
  <app-main></app-main>
  <app-nav></app-nav>
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>