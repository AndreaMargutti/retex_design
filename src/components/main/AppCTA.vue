<script>
export default {
  data() {
    return {
        name: 'AppCTA', 
    }
  }
}
</script>

<template>
    <div class="d-sm-flex justify-content-between align-items-center py-5">
        <h1>Il tuo supporto e fondamentale</h1>
        <p>
            Dai il tuo contributo
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-arrow-right" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8"/>
            </svg>
        </p>
    </div>
</template>

<style scoped lang="scss">

div {
    min-height: 150px;
    padding: 1.2rem;
    background-color: #f4f1de;
}

h1, p {
    font-weight: 600;
}
</style>