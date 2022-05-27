<template>
    <section id="projects">
      <div class="py-5 mb-5"></div>
      <v-container>
        <h6 class="text-center text-uppercase text-secondary fw-bold py-5" style="font-family: 'Montserrat', sans-serif">• Projects •</h6>
        <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif" data-aos="fade-up"  data-aos-easing="linear" data-aos-duration="900">My previous works</h1>
          <div class="row ">
            <div class="col-lg-12 col-sm-12 col-12">
              <div class="row">
                <div class="col-lg-6 col-md-6 col-sm-12 col-12 mb-5">
                  <v-hover v-slot="{ hover }">
                    <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="700" style="border-radius:20px;">
                    <v-img src="../assets/project.png" height="230px"></v-img>
                    <v-card-title class="text-centercard-title fw-bold">My Web Portfolio</v-card-title>
                    <v-card-subtitle class="fw-bold text-muted" style="font-family: 'Montserrat', sans-serif">Website / Web Application / Cloud Hosted</v-card-subtitle>
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
                        <v-card-subtitle class="fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif"><i class="fa-solid fa-earth-americas px-1"></i> May 20, 2022</v-card-subtitle>
                      </div>
                    </v-expand-transition>
                  </v-card>
                  </v-hover>
                </div>
                <div class="col-lg-6 col-md-6 col-sm-12 col-12 mb-5">
                  <v-hover v-slot="{ hover }">
                    <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="700" style="border-radius:20px;">
                      <v-img src="../assets/project1.png" height="230px"></v-img>
                      <v-card-title>Automated Class Grading System</v-card-title>
                      <v-card-subtitle class="fw-bold text-muted" style="font-family: 'Montserrat', sans-serif">Website / Progressive Web Application / System Software / Cloud Hosted</v-card-subtitle>
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
                          <v-card-text class="subtitle-2 text-justify">{{ about }}</v-card-text>
                          <v-card-subtitle class="fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif"><i class="fa-solid fa-earth-americas px-1"></i> May 24, 2022 - Integrative Programming and Technologies 3</v-card-subtitle>
                        </div>
                      </v-expand-transition>
                    </v-card>
                  </v-hover>
                </div>
              </div>
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
      about: 'An Automated Web-Based Class Grading System for the College of Information and Computing Science — making it easy, fast, reliable and User Friendly Web-Based System. Designed for Mobile Devices. Developed in PHP Laravel 9.10.',
      aboutMe: 'A Web Portfolio developed in Vue JS'
    }),
}
</script>