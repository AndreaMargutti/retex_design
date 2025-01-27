<script>
export default {
  data() {
    return {
        name: 'AppFooter',  
    }
  }
}
</script>

<template>
  <section class="d-flex justify-content-between align-items-center">
    <div>
      <ul class="d-flex gap-4">
        <li>Il Gruppo</li>
        <li>Note Legali</li>
        <li>Chi Siamo</li>
        <li>Condizioni d'uso</li>
        <li>Privacy</li>
        <li>Scrivici</li>
        <li>Pubblicita</li>
      </ul>
    </div>
    <div>
      <p>@1994-2022 Vita Societa Editoriale S.p.A.</p>
    </div>
  </section>
</template>

<style scoped lang="scss">
  section {
    min-height: 100px;
  }
</style>