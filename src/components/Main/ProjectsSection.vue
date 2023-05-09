<template>
  <section id="projects" class="py-lg-5 py-3">
    <div class="container rounded-5 title p-lg-5 p-4">
      <h2 class="fw-bold fs-1 mb-4 text-center">I Miei Progetti</h2>
      <span class="fw-bold fs-4 mb-4 d-block text-center">
        Ecco alcuni dei progetti che ho sviluppato. Clicca sul tasto Apri per
        vederne un anteprima.
      </span>
      <hr />
      <div class="row justify-content-around flex-wrap">
        <ProjectCard
          link="https://riccardo-bernardi-transport-company.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/proj-html-vuejs"
          class="col-lg-5 col-xl-3"
        >
          Sito di Trasporti
          <template v-slot:image>
            <img
              src="../../assets/img/Trasporti.png"
              class="card-img-top"
              alt="Immagine Sito di Trasporti"
            />
          </template>
          <template v-slot:description>
            Progetto in Vue.js va a creare un sito di una compagnia di
            trasporti.
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-boolflix.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/vite-boolflix"
          class="col-lg-5 col-xl-3"
        >
          Boolflix
          <template v-slot:image>
            <img
              src="../../assets/img/Netflix.png"
              class="card-img-top"
              alt="Immagine Progetto Boolflix"
            />
          </template>
          <template v-slot:description>
            Replica in Vue.js del noto servizio di streaming "Netflix".
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-dropbox.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/htmlcss-dropbox"
          class="col-lg-5 col-xl-3"
        >
          Dropbox
          <template v-slot:image>
            <img
              src="../../assets/img/Dropbox.png"
              class="card-img-top"
              alt="Immagine Progetto Dropbox"
            />
          </template>
          <template v-slot:description>
            Progettazione Front End di 'Dropbox' un diffuso servizio di file
            hosting.
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-spotify.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/html-css-spotifyweb"
          class="col-lg-5 col-xl-3"
        >
          Spotify
          <template v-slot:image>
            <img
              src="../../assets/img/Spoty.png"
              class="card-img-top"
              alt="Immagine Progetto Spotify"
            />
          </template>
          <template v-slot:description>
            Replica in HTML e CSS dell'app "Spotify".
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-boolzapp.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/vue-boolzapp"
          class="col-lg-5 col-xl-3"
        >
          <template v-slot:image>
            <img
              src="../../assets/img/Whatsapp.png"
              class="card-img-top"
              alt="Immagine Progetto WhatsApp"
            />
          </template>
          WhatsApp
          <template v-slot:description>
            Sviluppo tramite Vue.js dell' app "WhatsApp".
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-discord.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/htmlcss-discord"
          class="col-lg-5 col-xl-3"
        >
          Discord
          <template v-slot:image>
            <img
              src="../../assets/img/Discord.png"
              class="card-img-top"
              alt="Immagine Progetto Discord"
            />
          </template>
          <template v-slot:description>
            Sviluppo lato Front End dell' app "Discord".
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-bootstrap-dashboard.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/html-css-bootstrap-dashboard"
          class="col-lg-5 col-xl-3"
        >
          Bootstrap Dashboard
          <template v-slot:image>
            <img
              src="../../assets/img/dashboard.png"
              class="card-img-top"
              alt="Immagine Progetto Bootstrap Dashboard"
            />
          </template>
          <template v-slot:description>
            Dashboard sviluppata in html, css e bootstrap.
          </template>
        </ProjectCard>
        <ProjectCard
          link="https://riccardo-bernardi-campo-minato.netlify.app"
          gitLink="https://github.com/RiccardoBernardi1/campo-minato-1"
          class="col-lg-5 col-xl-3"
        >
          Campo Minato
          <template v-slot:image>
            <img
              src="../../assets/img/campo-minato.png"
              class="card-img-top"
              alt="Immagine Progetto Campo Minato"
            />
          </template>
          <template v-slot:description>
            Campo minato sviluppato con Vue.js. (Arriveranno presto dei
            miglioramenti)
          </template>
        </ProjectCard>
      </div>
      <hr class="mb-xl-5" />
      <div class="d-xl-flex">
        <div class="px-lg-5 col-xl-4">
          <div class="accordion d-lg-none" id="accordionExample">
            <div class="accordion-item">
              <h3 class="accordion-header mt-4 mb-4">
                <button
                  class="accordion-button collapsed fw-bold fs-2 text-center"
                  type="button"
                  data-bs-toggle="collapse"
                  data-bs-target="#collapseThree"
                  aria-expanded="false"
                  aria-controls="collapseThree"
                >
                  Video del Progetto "Replica Deliveroo"
                </button>
              </h3>
              <div
                id="collapseThree"
                class="accordion-collapse collapse"
                data-bs-parent="#accordionExample"
              >
                <div class="accordion-body">
                  <span class="fw-bold fs-4 text-center d-block mb-4"
                    >Questo video mostra brevemente la grafica e le principali
                    funzionalità del sito sviluppato dal team di cui ho fatto
                    parte come progetto finale del corso di Boolean.</span
                  >
                </div>
              </div>
            </div>
          </div>
          <div class="d-none d-lg-block">
            <h3 class="text-center mt-4 mb-4 fw-bold fs-2">
              Video Progetto Replica Deliveroo
            </h3>

            <span class="fw-bold fs-4 text-center d-block mb-4"
              >Questo video mostra brevemente la grafica e le principali
              funzionalità del sito sviluppato dal team di cui ho fatto parte
              come progetto finale del corso di Boolean.</span
            >
          </div>
        </div>
        <hr class="d-lg-none mb-4" />
        <div class="d-flex justify-content-center">
          <video
            src="../../assets/videos/2023-03-17-12-14-49.mp4"
            class="w-100 rounded-4"
            controls
          >
            Your browser does not support the video.
          </video>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ProjectCard from "./ProjectCard.vue";
export default {
  components: {
    ProjectCard,
  },
};
</script>

<style lang="scss" scoped>
#projects {
  background-color: rgba($color: #000000, $alpha: 0.4);
  .row > * {
    padding: 0;
  }
  hr {
    color: white;
  }
  .title {
    background-color: rgba($color: #000000, $alpha: 0.7);
    h2 {
      color: bisque;
      font-family: "Proza Libre", sans-serif;
    }
    span {
      color: whitesmoke;
    }
  }
  .accordion,
  .accordion > *,
  .accordion-button {
    background-color: transparent;
    color: inherit;
    border: none;
  }

  h3 {
    color: bisque;
    font-family: "Taviraj", serif;
  }
}
</style>
