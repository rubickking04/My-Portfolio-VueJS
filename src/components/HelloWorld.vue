<template>
  <section id="home">
    <v-container>
      <!-- <div class="py-5"> -->
        <div class="py-5">
          <div class="py-5">
            <v-row class="text-center py-5">
              <div class="mb-4 col-lg-6 col-md-8">
                <div class="py-5">
                  <div class="py-5">
                    <div class=" container">
                      <h3 class=" px-2 text-start font-weight-bold" style="font-family: 'Montserrat', sans-serif">Hello, I'm </h3>
                      <h1 class="my-text text-start font-weight-bold my-name" style="font-family: 'Poppins', sans-serif; font-size:50px;">{{ me }}</h1>
                      <vue-typed-js :strings="['System Analyst.','Programmer.','Fullstack Web Developer.' ]">
                        <p class="headline text-start font-weight-bold">I'm a <span class="typing text-info" style="font-family: 'Montserrat', sans-serif"></span></p>
                      </vue-typed-js>
                      <!-- <p class="headline text-start font-weight-bold">A <span class="text">Fullstack Web Developer.</span> </p> -->
                      <div class="text-start mb-3">
                        <a href="https://twitter.com/rubickking04"><span class="fs-1 bi bi-twitter text-info px-3"></span></a>
                        <a href="https://www.facebook.com/alfhaigar.usman.1/" ><span class="fs-1 px-3 bi bi-facebook text-primary"></span></a>
                        <a href="https://github.com/rubickking04"><span class="fs-1 px-3 bi bi-github text-dark"></span></a>
                        <a href="https://www.instagram.com/kingrubick_04/"><span class="fs-1 bi bi-instagram text-danger px-3"></span></a>
                        <a href="https://www.linkedin.com/in/al-fhaigar-usman-108812193/"><span class="fs-1 bi bi-linkedin text-primary px-3"></span></a>
                      </div>
                      <div class="text-start row no-gutters">
                        <div class="col-lg-3 col-md-3 col-sm-3 col-5">
                          <v-btn dark large  elevation="20" class="text-start" href="#about">About me</v-btn>
                        </div>
                        <div class="col-lg-3 col-md-3 col-sm-3 col-6">
                          <v-btn large class="text-start fw-bold"  elevation="15" href="#about" >Download CV</v-btn>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-lg-6 col-md-4 d-none d-md-block">
                <v-hover>
                  <img  src="../assets/me1.jpg" height="450" width="450" class="img-thumbnail rounded-circle border border-5 border-secondary" alt="...">
                </v-hover>
              </div>
            </v-row>
          </div>
        </div>
      <!-- </div> -->
    </v-container>
  </section>
</template>

<script>
export default {
  name: "HelloWorld",
  data: () => ({
    me: 'Al-Fhaigar Usman'
  }),
};
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');

</style>
