<script>
import AppCTA from './AppCTA.vue';
import MainArticle from './MainArticle.vue';
import ThreeArticle from './ThreeArticle.vue';

export default {
  data() {
    return {
     name: 'AppMain', 
    }
  },

  components: {
    MainArticle,
    ThreeArticle,
    AppCTA,
  }
}
</script>

<template>
  <MainArticle />
  <ThreeArticle />
  <!-- Inserisco componente CTA -->
  <AppCTA />

</template>

<style scoped lang="scss">

</style>