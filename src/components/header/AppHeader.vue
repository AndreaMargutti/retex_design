<script>
import AppLog from './AppLog.vue';
import AppNavbar from './AppNavbar.vue';

export default {
  data() {
    return {
     name: 'AppHeader', 
    }
  },
  components: {
    AppLog,
    AppNavbar,
  }
}
</script>

<template>
    <AppLog />
    <AppNavbar />
</template>

<style scoped lang="scss">
</style>