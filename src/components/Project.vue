<template>
    <section id="projects">
      <v-container>
        <h6 class="text-center text-uppercase text-secondary fw-bold py-5" style="font-family: 'Montserrat', sans-serif">• Projects •</h6>
        <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif">My previous works</h1>
          <div class="row py-5">
            <div class="col-lg-6 col-12">
              <v-hover v-slot="{ hover }">
                <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="500" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-easing="linear" data-aos-duration="900">
                <v-img src="../assets/project1.png" height="200px"></v-img>
                <v-card-title>College of Information and Computing Science</v-card-title>
                <v-card-subtitle class="subtitle-1">Automated Class Grading System</v-card-subtitle>
                <v-card-actions>
                  <v-btn href="https://zppsu-cics-wannabe.herokuapp.com/" color="orange lighten-2" text>Explore Now</v-btn>
                  <v-spacer></v-spacer>
                  <v-btn icon @click="show = !show">
                    <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                  </v-btn>
                </v-card-actions>
                <v-expand-transition>
                  <div v-show="show">
                    <v-divider></v-divider>
                    <v-card-text class="subtitle-2">{{ about }}</v-card-text>
                  </div>
                </v-expand-transition>
              </v-card>
              </v-hover>
              </div>
          </div>
        </v-container>
    </section>
</template>
<script>
export default {
    name: 'My-Ugly-Projects',
    data: () => ({
      show: false,
      about: 'A Web-Based Online Grading System for the students of College of Information and Computing Science — making it easy, fast, reliable and User Friendly Web-Based System. Designed for Mobile Devices.'
    }),
}
</script>