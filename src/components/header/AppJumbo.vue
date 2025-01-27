<script>
export default {
  data() {
    return {
     name:'AppJumbo', 
    }
  },

  props: {
    navItems: Array,
  }
}
</script>

<template>
    <section class="d-flex justify-content-between py-5 px-3">
        <h1>{{ navItems[0] }}</h1>
        <ul class="d-flex align-self-end">
            <li v-for="(item, index) in navItems" :key="item">
                <button v-if="index > 0">{{ item }}</button>
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

    ul {
        list-style-type: none;
    }

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

</style>