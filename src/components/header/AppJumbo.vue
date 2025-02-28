<script>
export default {
  data() {
    return {
     name:'AppJumbo',
    }
  },

  props: {
    navItems: Array,
  },
}
</script>

<template>
    <section class="navbar justify-content-between py-4 px-3">
        <h1 class="nav-item">{{ navItems[0] }}</h1>
        <ul class="nav-item d-flex gap-1 flex-wrap">
            <li v-for="(item, index) in navItems" :key="item" class="">
                <button v-if="index !== 0"
                    :class="{
                        // se i bottoni corrispono a certe categorie allora gli assegno una determinata classe
                        'btn-green': item === 'Ambiente',
                        'btn-red': item === 'Mondo',
                        'btn-bronze': item === 'Politica'
                    }"
                >
                    {{ item }}
                </button>
            </li>
        </ul>
    </section>
</template>

<style scoped lang="scss">

    section{
        background-color: #f4f4f4;
    }

    h1 {
        font-size: 2.5rem;
        font-weight: 700;
    }

    // lista

    li {
        padding-right: 1.2rem;
    }

    // bottoni

    button {
        background-color: white;
        padding: 0.5rem;
        border: 2px solid black;
        border-radius: 10px;
        box-shadow: -3px 3px ;
        text-transform: uppercase;
        font-weight: 600;
    }
    
    .btn-green {
        background-color: #e2f1e8;
    }

    .btn-red {
        background-color: #f1dada;
    }

    .btn-bronze {
        background-color: #f1f1e2;
    }

    // sezione responsive
    @media screen and (max-width: 576px) {
        ul , li{
            padding: 0;
            margin: 0;
        }

        button {
            background-color: white !important;
        }
    }

</style>