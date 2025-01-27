<script>
export default {
  data() {
    return {
        name: 'AppNavbar', 
    }
  },

  props: {
    navItems: Array
  }
}
</script>

<template>
  
  <!-- sezione menu -->
  <section class="d-flex justify-content-between">
    <!-- icona hamburger menu -->
    <div class="p-3">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16" color="red">
        <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
      </svg>
    </div>
    <div class="p-3">
      <!-- icona lente -->
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
        <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001q.044.06.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1 1 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0"/>
      </svg>
    </div>
  </section>

  <!-- sezione lista -->

  <section class="p-2">
    <ul class="d-flex gap-3">
      <li v-for="item in navItems">
        <h3>{{ item }}</h3>
      </li>
    </ul>
  </section>

</template>

<style scoped lang="scss">
  section {
    border-bottom: 2px solid black;
  }

  div {
    border-style: solid;
    border-width: 0px 1px 0px 1px;
}

// lista

ul {
  list-style-type: none;
  margin-bottom: 0;
  padding-left: 1.2rem;
}

h3 {
  font-weight: 600;
}

</style>