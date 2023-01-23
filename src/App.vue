<script>
import AppHeader from './components/AppHeader.vue';
import { headerLinks, comics } from './data/index.js'
export default {
  name: 'Comics Site',
  data() {
    return {
      headerLinks,
      comics
    }
  },
  components: {
    AppHeader,
  },
}
</script>

<template>
  <app-header :links="headerLinks"></app-header>

</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>