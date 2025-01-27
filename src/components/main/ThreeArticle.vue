<script>
export default {
  data() {
    return {
        name: 'ThreeArticle', 
    }
  }
}
</script>

<template>
    <section>
        <div id="long-article" class="d-flex flex-column justify-content-end">
            <p class="tag">ALLARMI</p>
            <h1>
                Il collasso dei ghiacciai negli scatti <br> 
                del fotografo ambientale Fabiano Ventura
            </h1>
            <figure>
                <img src="../../../public/d7312632d8e9cc247b26cdd7abe33d50.png" alt="">
                <div>
                    <h5>Di Ugo Lombi</h5>
                    <h6>14 Luglio 2022</h6>
                </div>
            </figure>
        </div>
        <div>
            <!-- TODO: inserire gli altri due articoli -->
        </div>
    </section>
</template>

<style scoped lang="scss">
#long-article {
    min-height: 700px;
    background-image: url(../../../public/6b12b5889d6ddad962a628409ed1fb35.png);
    background-size: cover;
    padding: 1.2rem;
}

.tag {
background-color: #e2f1e8;
width: fit-content;
padding: 10px;
border: 2px solid black;
border-radius: 10px;
box-shadow: -3px 3px;
}

h1 {
    color: white;
    font-weight: 600;
}

figure {
    color: white;
    margin-top: 25px;
    img {
      height: 50px;
      border-radius: 50%;
      margin-right: 25px;
    }
  }

</style>