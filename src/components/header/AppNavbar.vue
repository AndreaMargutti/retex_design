<script>
export default {
  data() {
    return {
        name: 'AppNavbar',
        // variabile per funzione operMenus e v-show
        list: true,
    }
  },

  props: {
    navItems: Array
  },

  methods: {
     openMenu () {
        // assegna alla varaiabile il suo valore opposto
        this.list = !this.list;
      }
  },
}
</script>

<template>
  
  <!-- sezione menu -->
  <section class="topic-list d-flex justify-content-between">
    <div class="p-3 border-div">
         <!-- icona hamburger menu -->
         <svg v-show="list" v-on:click="openMenu" xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16" color="red">
           <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
          </svg>
          <!-- icona X -->
          <svg v-show="!list" v-on:click="openMenu" xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-x" viewBox="0 0 16 16" color="red">
            <path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708"/>
          </svg>
    </div>
    
    <div v-show="list" class="p-3 border-div">
      <!-- icona lente -->
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16" color="red">
        <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001q.044.06.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1 1 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0"/>
      </svg>
    </div>
  </section>

  <!-- sezione lista -->
  <div v-show="list" class="topic-list">
    <section v-show="list" class="d-flex justify-content-between">
      <ul class="d-flex gap-3">
        <li v-for="item in navItems" class="pe-3">
          <h3>{{ item }}</h3>
        </li>
      </ul>

      <div class="d-flex align-items-center gap-1 pe-3">
        <h4>Aa</h4>
        <!-- image icon -->
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-image-fill" viewBox="0 0 16 16">
          <path d="M.002 3a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-12a2 2 0 0 1-2-2zm1 9v1a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V9.5l-3.777-1.947a.5.5 0 0 0-.577.093l-3.71 3.71-2.66-1.772a.5.5 0 0 0-.63.062zm5-6.5a1.5 1.5 0 1 0-3 0 1.5 1.5 0 0 0 3 0"/>
        </svg>
      </div>
    </section>
  </div>

  <!-- sezione hamburger menu -->

  <section id="hamburger" v-show="!list" class="border-bottom-0">
    <div class="row">
        <div class="col border border-dark ham-col">
          <h3>Articoli</h3>
          <p>Trend, dati e novita del Terzo Settore</p>
        </div>
        <div class="col border border-dark ham-col">
          <h3>Storie</h3>
          <p>Letture ed approfondimenti dei fenomeni complessi</p>
        </div>
        <div class="col border border-dark ham-col">
          <h3>Interviste</h3>
          <p>Racconti reali di persone ed organizzazioni</p>
        </div>
    </div>
    
    <div class="row">
      <div class="col border border-dark ham-col">
        <h3>Opinioni</h3>
        <p>Riflessioni e confronti dei nostri opinionisti</p>
      </div>
      <div class="col border border-dark ham-col">
        <h3>Podcast</h3>
        <p>Un luogo per dare voce ai protagonisti della sostenibilita</p>
      </div>
      <div class="col border border-dark ham-col">
        <h3>Bookazine</h3>
        <p>Una rivista da leggere e un libro da conservare</p>
      </div>
    </div>

    <div class="row">
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Chi siamo</h6>
      </div>
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Comitato Editoriale</h6>
      </div>
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Servizi</h6>
      </div>
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Agenda/Eventi</h6>
      </div>
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Mappa dell'attivismo</h6>
      </div>
      <div class="col border border-dark border-bottom-0 ham-ft">
        <h6>Inchieste crowdfunding</h6>
      </div>
    </div>
  </section>

</template>

<style scoped lang="scss">

.border-div {
  border-style: solid;
  border-width: 0px 1px 0px 1px;
}

// sezione lista

ul {
  margin-bottom: 0;
  padding-left: 1.2rem;
}

li {
  padding: 25px 0;
}

ul > :first-child {
  border-bottom: 10px solid red;
}

h3 {
  font-weight: 600;
}

h4 {
  margin-bottom: 0;
}

// sezione hamburger menu

.ham-col {
  height: 300px;
  padding: 25px;
  display: flex;
  flex-direction: column;
  justify-content: end;

  h3 {
    font-size: 2.5rem;
    font-weight: 800;
  }
}

.ham-ft {
  padding: 25px;
  text-align: center;
}

@media screen and (max-width: 576px) {
  .topic-list {
    display: none !important;
  }

  
}

</style>