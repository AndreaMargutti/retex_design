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
  <section class="row align-items-center">
    <div class="col-sm-9">
      <ul class="d-sm-flex gap-4">
        <li>Il Gruppo</li>
        <li>Note Legali</li>
        <li>Chi Siamo</li>
        <li>Condizioni d'uso</li>
        <li>Privacy</li>
        <li>Scrivici</li>
        <li>Pubblicita</li>
      </ul>
    </div>
    <div class="col-sm-3">
      <p>@1994-2022 Vita Societa Editoriale S.p.A.</p>
    </div>
  </section>
</template>

<style scoped lang="scss">
  section {
    min-height: 100px;
  }

@media screen and (max-width: 576px) {
  p{
    padding-left: 1.5rem;
  }


  ul {
    padding-top: 10px;
    padding-left: 1.5rem;
    li {
      font-weight: 700;
      font-size: 1.5rem;
      margin-bottom: 10px;
    }
  }
  
}
</style>