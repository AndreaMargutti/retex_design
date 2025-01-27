<script>
export default {
  data() {
    return {
     name: 'AppJumbo', 
    }
  },

  props: {
    navItems: Array,
  }
}
</script>

<template>
    <section>
        <h1>{{ navItems[0] }}</h1>
    </section>
</template>

<style scoped lang="scss">
</style>