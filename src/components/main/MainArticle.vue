<script>
export default {
  data() {
    return {
        name: 'MainArticle', 
    }
  }
}
</script>

<template>
  <section>
    <div class="d-flex flex-column justify-content-end" id="main">
        <div id="article">
          <p class="tag">MIGRANTI</p>
          <h1>
            Roccella Jonica, la Lampedusa che  <br>
            l'Italia ignora
          </h1>
          <figure class="d-flex">
            <img src="../../../public/e059a7a3367ff920d07e1938b4e8cd8f.jpeg" alt="profile-pic">
            <div>
              <h5>Di Alessandro Puglia</h5>
              <h6>29 giugno 2022</h6>
            </div>
          </figure>
        </div>
      </div>
  </section>
</template>

<style scoped lang="scss">
  section {
    border: 0;
  }

  #main {
    min-height: 600px;
    background-image: url(../../../public/44146596a39e532d863a717f24411c63.jpeg);
    background-size: cover;
    padding: 1.2rem;
  }

  .tag {
    background-color: white;
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

  @media screen and (max-width: 576px) {
    #main {
      min-height: 100%;
      background-position: center;
      background-repeat: no-repeat;
      padding: 1.5rem;
    }

    #article {
      margin-top: 150px;
    }
  }
</style>