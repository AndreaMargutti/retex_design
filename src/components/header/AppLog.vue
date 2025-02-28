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
    <section class="row p-md-3 justify-content-between">
      <div class="col d-flex text-center text-md-start">
        <div id="contr" class="flex-grow-1 flex-md-grow-0 py-2 py-md-0">Contribuisci</div>
        <div class="flex-grow-1 flex-md-grow-0 ps-4 py-2 py-md-0">Abbonati</div>
      </div>
      <!-- Sezione Accesso -->
      <div class="col-md-6 d-md-flex justify-content-end d-none d-sm-none">
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
    #contr {
      border: solid black;
      border-width: 0 2px 0 0;
    }
}
</style>