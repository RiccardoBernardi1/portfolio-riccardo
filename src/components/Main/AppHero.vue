<template>
  <section id="hero" class="pb-lg-0 pb-3 pt-2 pt-lg-4">
    <div class="container d-xl-flex align-items-start d-none">
      <img src="../assets/img/Riccardo-2.png" alt="Riccardo" />
      <div class="col-right p-4 rounded-4 mb-5">
        <h1 class="fw-bold mb-4">
          Ciao, mi chiamo Riccardo e sono un Full Stack Web Developer Jr
        </h1>
        <span class="fs-4"
          >Questo ambiente dinamico e sempre in crescita mi spinge costantemente
          a superare i miei limiti. Conoscere e approfondire nuove entusiasmanti
          tecnologie in continuo mutamento offre la possibilità di crescere, sia
          a livello lavorativo che a livello personale e io sono pronto a
          coglierla!</span
        >
      </div>
    </div>
    <div class="container d-xl-none container-fluid">
      <div class="col-right px-md-5 p-4 py-lg-5 rounded-4">
        <h1 class="fw-bold mb-md-4 mb-4">
          Ciao, mi chiamo Riccardo e sono un Full Stack Web Developer Jr
        </h1>
        <div class="d-md-flex align-items-center">
          <img
            src="../assets/img/Riccardo-2.png"
            alt="Riccardo"
            class="ms-image"
          />
          <span class="fs-4"
            >Questo ambiente dinamico e sempre in crescita mi spinge
            costantemente a superare i miei limiti. Conoscere e approfondire
            nuove entusiasmanti tecnologie in continuo mutamento offre la
            possibilità di crescere, sia a livello lavorativo che a livello
            personale e io sono pronto a coglierla!</span
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#hero {
  .container {
    padding-top: 4.25rem;
    @media screen and (min-width: 992px) {
      min-height: 100vh;
    }
    .ms-image {
      margin-bottom: -3rem;
      @media screen and (max-width: 992px) {
        display: none;
      }
      &.w-100 {
        max-width: 100%;
      }
    }
    img {
      max-height: 100%;
      max-width: 60%;
      margin-top: auto;
    }
    .col-right {
      background-color: rgba($color: #000000, $alpha: 0.5);

      box-shadow: #000000 5px 5px 20px 10px;
      h1 {
        color: bisque;

        font-family: "Taviraj", serif;
        @media screen and (min-width: 992px) {
          font-size: 50px;
        }
      }
      span {
        color: white;
      }
    }
  }
}
</style>
