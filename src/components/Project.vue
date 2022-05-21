<template>
    <section id="projects">
      <v-container>
        <h6 class="text-center text-uppercase text-secondary fw-bold py-5" style="font-family: 'Montserrat', sans-serif">• Projects •</h6>
        <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-easing="linear" data-aos-duration="900">My previous works</h1>
          <div class="row py-5 no-gutters">
            <div class="col-lg-6 col-md-6 col-sm-12 col-12 mb-5">
              <v-hover v-slot="{ hover }">
                <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="550">
                <v-img src="../assets/project2.png" height="230px"></v-img>
                <v-card-title>My Web Portfolio</v-card-title>
                <v-card-subtitle class="subtitle-1 fw-bold">Al-Fhaigar Usman</v-card-subtitle>
                <v-card-text><v-btn href="https://vuejs.org/" elevation="2" large outlined color="#1b5e20" ><i class="fa-brands font-weight-bold fs-4 fa-vuejs px-2" style="color:#1b5e20;"></i>Vue JS</v-btn></v-card-text>
                <v-card-actions>
                  <v-btn href="https://alfhaigarusman04.herokuapp.com/" color="#1b5e20" text>Explore Now</v-btn>
                  <v-spacer></v-spacer>
                  <v-btn icon @click="shaw = !shaw">
                    <v-icon>{{ shaw ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                  </v-btn>
                </v-card-actions>
                <v-expand-transition>
                  <div v-show="shaw">
                    <v-divider></v-divider>
                    <v-card-text class="subtitle-2">{{ aboutMe }}</v-card-text>
                  </div>
                </v-expand-transition>
              </v-card>
              </v-hover>
            </div>
            <div class="col-lg-6 col-md-6 col-sm-12 col-12 mb-5">
              <v-hover v-slot="{ hover }">
                <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="550">
                <v-img src="../assets/project1.png" height="230px"></v-img>
                <v-card-title>System Software</v-card-title>
                <v-card-subtitle class="subtitle-1 fw-bold" style="font-family: 'Montserrat', sans-serif">CICS - Automated Class Grading System</v-card-subtitle>
                <v-card-text><v-btn href="https://laravel.com/" elevation="2" large outlined color="red" ><i class="fa-brands font-weight-bold fs-4 fa-laravel px-2" style="color:red;"></i>laravel</v-btn></v-card-text>
                <v-card-actions>
                  <v-btn href="https://zppsu-cics-wannabe.herokuapp.com/" color="red" text>Explore Now</v-btn>
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
      shaw: false,
      about: 'A Web-Based Online Grading System for the students of College of Information and Computing Science — making it easy, fast, reliable and User Friendly Web-Based System. Designed for Mobile Devices.',
      aboutMe: 'Hi, My name is Al-Fhaigar J. Usman a Fullstack Developer and a System Analyst from Zamboanga City, Philippines. I create a custom website to help everyone do better online, I am currently studying as a 3rd year student at Zamboanga Peninsula Polytechnic State University.'
    }),
}
</script>