<template>
    <section id="about">
        <div class="py-5 mb-5"></div>
        <v-container>
            <div class="py-5">
                <div class="py-5">
                    <div class="row justify-content-center ">
                        <v-row class="col-lg-12">
                            <v-card elevation="12" shaped >
                                <v-card-body class="card-body">
                                    <div class="row g-0">
                                        <div class="col-md-4">
                                            <img  src="../assets/me1.jpg" class="img-thumbnail rounded-start border border-5 border-secondary" alt="...">
                                            
                                        </div>
                                        <div class="col-md-8">
                                            <div class="card-body">
                                                <v-card-title class="display-2 fw-bold">About Me</v-card-title>
                                                <!-- <vue-typed-js :strings="['System Analyst.','Programmer.','System Developer.','Fullstack Web Developer.' ]"  @onComplete="doSmth()" :typeSpeed="50" :loop="true" :backSpeed="60" :startDelay="1000">
                                                    <v-card-subtitle class="title font-weight-bold" style="font-family: 'Montserrat', sans-serif;">I'm a <span class="typing"  style=" color:#0277BD;"></span></v-card-subtitle>
                                                </vue-typed-js> -->
                                                <v-card-subtitle class=" title text-primary fw-bold">Fullstack Developer & System Analyst</v-card-subtitle>
                                                <v-card-text class="subtitle-1">{{ aboutMe }}</v-card-text>
                                                <div class="row no-gutters">
                                                    <div class="col-lg-2 col-md-3 col-sm-3 col-5">
                                                        <v-btn href="#contact" elevation="12" dark class="mx-4 mb-2">Hire Me</v-btn>
                                                    </div>
                                                    <div class="col-lg-3 col-md-6 col-sm-6 col-6">
                                                        <v-btn elevation="12" @click="downloadFile" class="mx-2 fw-bold mb-2">Download CV</v-btn>
                                                    </div>
                                                </div>
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
import download from 'downloadjs';
export default {
    name: "About-Me-Myself-and-i",
    data: () => ({
        aboutMe: 'Hi, My name is Al-Fhaigar J. Usman a Fullstack Developer and a System Analyst from Zamboanga City, Philippines. I create a custom website to help everyone do better online, I am currently studying as a 3rd year student at Zamboanga Peninsula Polytechnic State University. If you are an employer looking for hire you can get in touch with me here.'
    }),
    methods: {
        downloadFile() {
            const url = '../assets/Al-Fhaigar Usman - Resume-v2.pdf';
            download(url);
            // const link = document.createElement('a');
            // link.href = url;
            // link.download = 'Al-Fhaigar Usman - Resume-v2.pdf';
            // document.body.appendChild(link);
            // link.click();
            // document.body.removeChild(link);
        }
    }
}
</script>