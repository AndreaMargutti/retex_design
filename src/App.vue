<script>
import AppHeader from './components/header/AppHeader.vue';
import AppMain from './components/main/AppMain.vue';

export default {
  data() {
    return {
      
    }
  },
  
  components: {
    AppHeader,
    AppMain,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
</template>

<style lang="scss">
  // importo bootstrap
  @use  '../node_modules/bootstrap/scss/bootstrap.scss' as *;
  // importo il foglio generale
  @use './style/general.scss' as *;
</style>