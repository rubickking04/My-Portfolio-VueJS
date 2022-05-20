<template>
    <section id="services" class="py-5">
        <v-container>
            <h6 class="text-center text-uppercase text-secondary fw-bold" style="font-family: 'Montserrat', sans-serif">• Services •</h6>
            <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif">What i do</h1>
            <div class="row justify-content-center" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-easing="linear" data-aos-duration="600">
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <div class="py-2">
                                    <v-img src="../assets/web.png" height="250px"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class=" fw-bold">01. Website</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A 100% Responsive Web Design for your business.</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center text-capitalize title mb-5" rounded large>Contact now! <i class="fa-solid px-3 fs-4 fa-circle-arrow-right"></i></v-btn>
                                </div>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <div class="py-2">
                                    <v-img src="../assets/web1.png" height="250px"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class=" fw-bold">Web Application</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">Reach your users in a user-friendly web application.</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center text-capitalize title mb-5" rounded large style="font-family: 'Montserrat', sans-serif">Contact now! <i class="fa-solid px-3 fs-4 fa-circle-arrow-right"></i></v-btn>
                                </div>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <div class="py-2">
                                    <v-img src="../assets/web3.png" height="250px"></v-img>
                                </div>                                
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="fw-bold">Mobile Application</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A hassle-free access with their mobile phones.</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center text-capitalize title mb-5" rounded large>Contact now! <i class="fa-solid px-3 fs-4 fa-circle-arrow-right"></i></v-btn>
                                </div>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
            </div>
        </v-container>
    </section>
</template>
<script>
export default {
    name: 'My-Services-in-work'
}
</script>