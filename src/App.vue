<template>
  <v-app>
      <nav class="navbar navbar-expand-lg navbar-dark bg-dark shadow sticky-top">
        <div class="container">
          <a href="https://alfhaigarusman04.herokuapp.com/" class="d-flex navbar-brand">
            <v-img
              alt="Vuetify Logo"
              class="shrink px-1"
              contain
              src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
              transition="scale-transition"
              width="30"
            />
            <v-img
              alt="Vuetify Name"
              class="shrink mt-1 hidden-sm-and-down px-4"
              contain
              min-width="80"
              src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
              transition="scale-transition"
              width="80"
            />
          </a>
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
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  id="no-background-hover"
                  href="#home"
                  text
                  class="text-white"
                  >Home</v-btn
                >
              </li>
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  href="#about"
                  id="no-background-hover"
                  text
                  class="text-white"
                  >About</v-btn
                >
              </li>
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  href="#services"
                  id="no-background-hover"
                  text
                  class="text-white"
                  >Services</v-btn
                >
              </li>
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  href="#skill"
                  id="no-background-hover"
                  text
                  class="text-white"
                  >Skills</v-btn
                >
              </li>
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  href="#projects"
                  id="no-background-hover"
                  text
                  class="text-white"
                  >Projects</v-btn
                >
              </li>
              <li class="nav-item mx-auto px-3 list-link">
                <v-btn
                  id="no-background-hover"
                  href="#contact"
                  text
                  class="text-white"
                >
                  Contact</v-btn
                >
              </li>
            </ul>
          </div>
        </div>
      </nav>
    <v-main>
      <HelloWorld />
      <About />
      <Services />
      <Skills />
      <Project />
      <Contact />
    </v-main>
    <v-footer dark padless class="copyright py-2 text-center fs-6 ">
    
      <div class="container fs-6 text-capitalize" style="font-family: 'Montserrat', sans-serif">
        <!-- <h1 class=" text-center  py-1 fw-bolder" style="font-family: 'Montserrat', sans-serif">Al-Fhaigar Usman</h1>
          <div class="text-center mb-3">
            <a href="https://www.facebook.com/alfhaigar.usman.1/" ><span class="fs-1 px-2 bi bi-facebook"></span></a>
            <a href="https://github.com/rubickking04"><span class="fs-1 px-2 bi bi-github px-2 text-light"></span></a>
            <a href="https://www.instagram.com/kingrubick_04/"><span class="fs-1 bi bi-instagram px-2 text-danger"></span></a>
          </div> -->
        © Created with a
        <lord-icon
          src="https://cdn.lordicon.com/rjzlnunf.json"
          trigger="loop"
          colors="primary:#f44336,secondary:#ffffff"
          stroke="100"
          style="width: 35px; height: 35px"
        >
        </lord-icon>
        by <a href="https://alfhaigarusman04.herokuapp.com/" class="text-decoration-none fw-bold ">Al-Fhaigar Usman</a>. All
        rights reserved 2022.
      </div>
    </v-footer>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import About from "./components/About.vue";
import Contact from "./components/Contact";
import Skills from "./components/Skills";
import Services from "./components/Services";
import Project from "./components/Project";

export default {
  name: "App",
  components: {
    HelloWorld,
    About,
    Contact,
    Skills,
    Project,
    Services,
  },

  data: () => ({
    model: null,
    classes: [
      ["h1", "Heading 1", "6rem", "300", "-.015625em", -1],
      ["h2", "Heading 2", "3.75rem", "300", "-.0083333333em", 0],
      ["h3", "Heading 3", "3rem", "400", "normal", 1],
      ["h4", "Heading 4", "2.125rem", "400", ".0073529412em", 2],
      ["h5", "Heading 5", "1.5rem", "400", "normal", 2],
      ["h6", "Heading 6", "1.25rem", "500", ".0125em", 3],
      ["subtitle-1", "Subtitle 1", "1rem", "400", ".009375em", 4],
      ["subtitle-2", "Subtitle 2", "0.875rem", "500", ".0071428571em", 4],
      ["body-1", "Body 1", "1rem", "400", ".03125em", 4],
      ["body-2", "Body 2", "0.875rem", "400", ".0178571429em", 4],
      ["button", "Button", "0.875rem", "500", ".0892857143em", 4],
      ["caption", "Caption", "0.75rem", "400", ".0333333333em", 4],
      ["overline", "Overline", "0.75rem", "500", ".1666666667em", 4],
    ],
  }),
};
</script>
<style lang="scss" scoped>
v-footer p .me-class {
  font-family: "Montserrat", sans-serif;
}
.list-link {
  font-family: "Montserrat", sans-serif;
  font-size: 20px;
  padding: 0 10px;
  display: inline-block;
  position: relative;
  color: #0087ca;
}
.list-link:hover {
  color: white;
  /* text-decoration: underline; */
}
.list-link::after {
  content: "";
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 4px;
  bottom: 0;
  left: 0;
  border-radius: 20px;
  background-color: white;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}
.list-link:hover::after {
  transform: scaleX(1);
  transform-origin: bottom left;
}
#no-background-hover::before {
  background-color: transparent !important;
}
</style>
