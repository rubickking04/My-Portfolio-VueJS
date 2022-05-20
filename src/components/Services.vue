<template>
    <section id="services">
        <v-container>
            <h6 class="text-center text-uppercase text-secondary fw-bold py-5" style="font-family: 'Montserrat', sans-serif">• Services •</h6>
            <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif">What i do</h1>
            <div class="row">
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <div class="py-2">
                                    <v-img src="../assets/web.png" height="200px"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="text-uppercase fw-bold">01. Website</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A stunning and Responsive Web Design for your business</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center title mb-3" rounded large>Contact now! <i class="fa-solid px-2 fs-4 fa-circle-arrow-right"></i></v-btn>
                                </div>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <div class="py-2">
                                    <v-img src="../assets/web1.png" height="200px"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="text-uppercase fw-bold">02. Web Application</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A stunning and Responsive Web Design for your business</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center title mb-3" rounded large>Contact now! <i class="fa-solid px-2 fs-4 fa-circle-arrow-right"></i></v-btn>
                                </div>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 2" :class="{ 'on-hover': hover  }" max-width="500">
                            <v-card-body class="text-center"> 
                                <v-img src="../assets/web.png" height="200px"></v-img>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h2 class="text-uppercase fw-bold">01. Website</h2></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A stunning and Responsive Web Design for your business</v-card-subtitle>
                                <div class="text-center">
                                    <v-btn href="#contact" dark class="text-center title mb-3" rounded large>Contact now! <i class="fa-solid px-2 fs-4 fa-circle-arrow-right"></i></v-btn>
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