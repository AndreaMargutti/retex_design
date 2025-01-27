<script>
import AppJumbo from './AppJumbo.vue';
import AppLog from './AppLog.vue';
import AppNavbar from './AppNavbar.vue';

export default {
  data() {
    return {
     name: 'AppHeader',

     navItems: [
        'Tutti i temi',
        'Ambiente',
        'Economia',
        'Mondo',
        'Non Profit',
        'Politica',
        'Società',
        'Welfare'
     ]
    }
  },
  
  components: {
    AppLog,
    AppNavbar,
    AppJumbo,
  }
}
</script>

<template>
    <AppLog />
    <AppNavbar :navItems="navItems"/>
    <AppJumbo :navItems="navItems"/>
</template>

<style scoped lang="scss">
</style>