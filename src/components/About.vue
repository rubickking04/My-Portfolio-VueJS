<template>
    <section id="about">
        <v-container>
            <div class="py-5">
                <div class="py-5">
                    <div class="row justify-content-center ">
                        <v-row class="col-lg-12">
                            <v-card elevation="12" shaped data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-easing="linear" data-aos-duration="900">
                                <v-card-body class="card-body">
                                    <div class="row g-0">
                                        <div class="col-md-4">
                                            <img  src="../assets/me1.jpg" class="img-thumbnail rounded-start border border-5 border-secondary" alt="...">
                                            
                                        </div>
                                        <div class="col-md-8">
                                            <div class="card-body">
                                                <v-card-title class="display-2 fw-bold">About Me</v-card-title>
                                                <v-card-subtitle class="title fw-bold">Fullstack Developer & System Analyst</v-card-subtitle>
                                                <v-card-text class="subtitle-1">{{ aboutMe }}</v-card-text>
                                                <v-btn elevation="12" dark class="mx-4">Hire Me</v-btn>
                                                <v-btn elevation="12"  class="mx-2 fw-bold">Download CV</v-btn>
                                            </div>
                                        </div>
                                    </div>
                                </v-card-body>
                            </v-card>
                        </v-row>
                    </div>
                </div>
            </div>
        </v-container>
    </section>
    
</template>
<script>
export default {
    name: "About-Me-Myself-and-i",
    data: () => ({
        aboutMe: 'Hi, My name is Al-Fhaigar J. Usman a Fullstack Developer and a System Analyst from Zamboanga City, Philippines. I create a custom website to help everyone do better online, I am currently studying as a 3rd year student at Zamboanga Peninsula Polytechnic State University.'
    }),
}
</script>