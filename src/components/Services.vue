<template>
    <section id="services" class="py-5">
        <div class="py-5 mb-5"></div>
        <v-container>
            <h6 class="text-center text-uppercase text-secondary fw-bold" style="font-family: 'Montserrat', sans-serif">• Services •</h6>
            <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif">What i do</h1>
            <div class="row justify-content-center" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-easing="linear" data-aos-duration="600">
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="1000" style="border-radius:20px;">
                            <v-card-body class="text-center"> 
                                <div class="mb-2 container">
                                    <v-img src="../assets/web4.png" height="200px" style="border-radius:20px;"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class=" fw-bold">Website</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A 100% Responsive Web Design for your business.</v-card-subtitle>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="1000" style="border-radius:20px;">
                            <v-card-body class="text-center"> 
                                <div class="mb-2 container">
                                    <v-img src="../assets/web5.png" height="200px" style="border-radius:20px;"></v-img>
                                </div>
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class=" fw-bold">Web Application</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">Reach your users in a user-friendly web application.</v-card-subtitle>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-4 col-md-4 col-sm-12 col-12">
                    <v-hover v-slot="{ hover }">
                        <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="1000" style="border-radius:20px;">
                            <v-card-body class="text-center"> 
                                <div class="mb-2 container">
                                    <v-img src="../assets/web3.png" height="200px" style="border-radius:20px;"></v-img>
                                </div>                                
                                <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="fw-bold">Mobile Application</h3></div>
                                <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A hassle-free access with their mobile phones.</v-card-subtitle>
                            </v-card-body>
                        </v-card>
                    </v-hover>
                </div>
                <div class="col-lg-8 col-md-8">
                    <div class="row">
                        <div class="col-lg-6 col-md-6 col-sm-12 col-12">
                            <v-hover v-slot="{ hover }">
                                <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="1000" style="border-radius:20px;">
                                    <v-card-body class="text-center"> 
                                        <div class="mb-2 container">
                                            <v-img src="../assets/web6.png" height="200px" style="border-radius:20px;"></v-img>
                                        </div>                                
                                        <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="fw-bold">System Software</h3></div>
                                        <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">A PHP Laravel and Vue JS integrated system software.</v-card-subtitle>
                                    </v-card-body>
                                </v-card>
                            </v-hover>
                        </div>
                        <div class="col-lg-6 col-md-6 col-sm-12 col-12">
                            <v-hover v-slot="{ hover }">
                                <v-card  :elevation="hover ? 24 : 5" :class="{ 'on-hover': hover  }" max-width="1000" style="border-radius:20px;">
                                    <v-card-body class="text-center"> 
                                        <div class="mb-2 container">
                                            <v-img src="../assets/web7.png" height="200px" style="border-radius:20px;"></v-img>
                                        </div>                                
                                        <div class="card-title font-weight-bold " style="font-family: 'Montserrat', sans-serif"><h3 class="fw-bold">Cloud Hosting</h3></div>
                                        <v-card-subtitle class="subtitle-1 fw-bold text-secondary" style="font-family: 'Montserrat', sans-serif">Hosting projects through Github Pages, Heroku, and more.</v-card-subtitle>
                                    </v-card-body>
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
    name: 'My-Services-in-work'
}
</script>
<style>
</style>