<template>
  <nav class="container justify-content-between pt-3 d-none d-lg-flex">
    <ul class="d-flex">
      <li>
        <a href="#" class="text-decoration-none fs-5 pe-3">Home</a>
      </li>
      <li>
        <a href="#hero" class="text-decoration-none fs-5 px-3">About Me</a>
      </li>
      <li>
        <a href="#projects" class="text-decoration-none fs-5 px-3">Progetti</a>
      </li>
      <li>
        <a href="#contact" class="text-decoration-none fs-5 px-3">Contatti</a>
      </li>
      <li>
        <a href="#" class="text-decoration-none fs-5 px-3" @click="download()"
          >Visualizza CV</a
        >
      </li>
    </ul>
    <ul class="d-flex">
      <li>
        <a
          href="https://www.linkedin.com/in/riccardo-bernardi/?profileId=ACoAAEDn5b0BNBVCoqdCLUAN4S7EngeuxHlxVbY"
          class="px-2 text-decoration-none fw-bold fs-4"
          ><i class="fa-brands fa-linkedin"></i
        ></a>
      </li>
      <li>
        <a
          href="https://github.com/RiccardoBernardi1?tab=repositories"
          class="ps-2 text-decoration-none fw-bold fs-4"
          ><i class="fa-brands fa-github"></i
        ></a>
      </li>
    </ul>
  </nav>
  <nav class="navbar navbar-expand-lg bg-body-tertiary navbar-dark d-lg-none">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <ul class="d-flex mb-0 px-0">
        <li>
          <a
            href="https://www.linkedin.com/in/riccardo-bernardi/?profileId=ACoAAEDn5b0BNBVCoqdCLUAN4S7EngeuxHlxVbY"
            class="px-2 text-decoration-none fw-bold fs-2"
            ><i class="fa-brands fa-linkedin"></i
          ></a>
        </li>
        <li>
          <a
            href="https://github.com/RiccardoBernardi1?tab=repositories"
            class="ps-2 text-decoration-none fw-bold fs-2"
            ><i class="fa-brands fa-github"></i
          ></a>
        </li>
      </ul>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#hero">About Me</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#projects">Progetti</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Contatti</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" @click="download()">Visualizza CV</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import CV from "../assets/pdf/CV_Riccardo_Bernardi.pdf";
export default {
  methods: {
    download() {
      window.location.href = CV;
    },
  },
};
</script>

<style lang="scss" scoped>
li {
  color: white;
  list-style: none;
  &:hover {
    color: #b990f7;
  }
  a {
    display: block;
    height: 100%;
    color: inherit;
  }
}
</style>
