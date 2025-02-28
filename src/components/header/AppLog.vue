<script>
export default {
  data() {
    return {
        name: 'AppLog', 
    }
  }
}
</script>

<template>
    <section class="d-flex p-3 justify-content-between">
    <div>Contribuisci</div>
    <div class="flex-fill ps-4">Abbonati</div>
    <!-- Sezione Accesso -->
    <div class="log">
      <!-- Icona (bootstrap-icon) -->
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-person" viewBox="0 0 16 16">
        <path d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6m2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0m4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4m-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10s-3.516.68-4.168 1.332c-.678.678-.83 1.418-.832 1.664z"/>
      </svg>
      Accedi
    </div>
  </section>
</template>

<style scoped lang="scss">
  @media screen and (max-width: 576px) {
    .log{
      display: none;
    }
    section {
      padding: 0px !important;
      text-align: center;
      border: solid black;
      border-width: 1px 0px;
      div {
        padding: 10px;
        border: solid black;
        border-width: 0px 0.5px 0px 0px;
        flex-basis: 50%;
        align-items: stretch;
      }
  }

  .flex-fill {
    flex: 50% !important;
  }
  

  }
</style>