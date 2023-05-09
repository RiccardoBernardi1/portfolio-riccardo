<template>
  <section id="contact" class="py-lg-5 py-3">
    <h2 class="fs-1 fw-bold text-center mb-lg-5 mb-4">Contattami</h2>
    <div
      class="container d-lg-flex justify-content-around align-items-start mb-lg-5 mb-3"
    >
      <div class="col-left px-lg-5 p-4 rounded-5 fw-bold mb-5 mb-lg-0">
        <h3 class="text-center mb-4 fs-2">Invia un messaggio</h3>
        <hr />
        <span class="fs-4 mb-4 d-block">
          Scrivimi un messaggio compilando questo form e risponderò il prima
          possibile via mail.
        </span>
        <hr />
        <form ref="form" @submit.prevent="sendEmail">
          <input type="hidden" name="contact_number" />
          <div class="mb-3">
            <label for="name" class="form-label">Nome</label>
            <input
              type="text"
              class="form-control"
              id="name"
              name="user_name"
              required
            />
          </div>
          <div class="mb-3">
            <label for="exampleInputEmail1" class="form-label">Email </label>
            <input
              type="email"
              class="form-control"
              id="Email"
              name="user_email"
              required
            />
          </div>
          <div class="mb-3">
            <label for="message" class="form-label">Messaggio</label>
            <textarea
              name="message"
              id="message"
              rows="5"
              class="form-control"
              required
            ></textarea>
          </div>
          <input type="submit" value="Invia" class="btn btn-success me-2" />
        </form>
      </div>
      <div class="col-right fs-4 fw-bold p-lg-5 p-4 rounded-5">
        <h3 class="mb-4 text-center fs-2">Altri contatti</h3>
        <hr />
        <ul>
          <li class="mb-4">
            <div class="mb-2">Mail :</div>
            <span>rikyb3004@gmail.com</span>
          </li>
          <li class="mb-4">
            <div class="mb-2">Tel :</div>
            <span>+39 3515360646</span>
          </li>
          <li>
            <div class="mb-2">Linkedin :</div>
            <a
              href="https://www.linkedin.com/in/riccardo-bernardi/?profileId=ACoAAEDn5b0BNBVCoqdCLUAN4S7EngeuxHlxVbY"
              >www.linkedin.com/in/riccardo-bernardi</a
            >
          </li>
        </ul>
        <hr />
      </div>
    </div>
    <div class="toast-container position-fixed bottom-0 end-0 p-3">
      <div
        id="liveToast"
        class="toast"
        role="alert"
        aria-live="assertive"
        aria-atomic="true"
      >
        <div class="toast-header">
          <strong class="me-auto">Messaggio Inviato</strong>
          <small>{{ new Date().toLocaleString() }}</small>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="toast"
            aria-label="Close"
          ></button>
        </div>
        <div class="toast-body">
          Ciao {{ username }}, il tuo messaggio è stato inviato con successo.
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import emailjs from "@emailjs/browser";
export default {
  data() {
    return {
      username: "",
    };
  },
  methods: {
    sendEmail() {
      this.username = this.$refs.form[1].value;
      emailjs
        .sendForm(
          "service_18qxoxk",
          "template_bkjw4hn",
          this.$refs.form,
          "oFcNV70jTpwBca2Op"
        )
        .then(
          (result) => {
            console.log("SUCCESS!", result.text);
            this.$refs.form.reset();
            let toast = document.getElementById("liveToast");
            toast.classList.add("show");
            setTimeout(() => toast.classList.remove("show"), 10000);
          },
          (error) => {
            console.log("FAILED...", error.text);
          }
        );
    },
  },
};
</script>

<style lang="scss" scoped>
h2 {
  color: bisque;
  font-family: "Proza Libre", sans-serif;
}
h3 {
  font-family: "Taviraj", serif;
}
.col-left {
  @media screen and (min-width: 992px) {
    max-width: 45%;
    min-width: 35%;
  }

  background-color: rgba($color: #490c29, $alpha: 0.8);
  box-shadow: #490c29 5px 5px 20px 10px;
  color: thistle;
}
.col-right {
  background-color: rgba($color: #000000, $alpha: 0.8);
  box-shadow: #000000 5px 5px 20px 10px;
  color: bisque;

  @media screen and (min-width: 992px) {
    max-width: 40%;
  }
  ul {
    padding-left: 0;
    li {
      list-style: none;
      a {
        text-decoration: none;
      }
    }
  }
}
</style>
