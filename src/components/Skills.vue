<template>
    <section id="skill">
        <div class="py-5 mb-5"></div>
        <v-container>
            <h6 class="text-center text-uppercase text-secondary fw-bold py-5" style="font-family: 'Montserrat', sans-serif">• Skills •</h6>
            <h1 class="text-center text-capitalize fw-bold py-5" style="font-family: 'Montserrat', sans-serif">My skills in programming</h1>
            <div class="row justify-content-center py-5">
                <div class="col-lg-12">
                    <div class="row no-gutters">
                        <div class="col-lg-6 col-md-6">
                            <v-container>
                                <p class="small text-uppercase fw-bold">Html 5</p>
                                <v-progress-linear v-model="html" color="deep-orange" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong >{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                                <p class="small text-uppercase fw-bold">Css 3</p>
                                <v-progress-linear v-model="css" color="light-blue" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong>{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                                <p class="small text-uppercase fw-bold">javascript</p>
                                <v-progress-linear v-model="js" color="yellow darken-2" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong>{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                            </v-container>
                        </div>
                        <div class="col-lg-6 col-md-6">
                            <v-container>
                                <p class="small text-uppercase fw-bold">bootstrap 5.1</p>
                                <v-progress-linear v-model="boot" color="indigo" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong>{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                                <p class="small text-uppercase fw-bold">PHP LAravel 9.10</p>
                                <v-progress-linear v-model="laravel" color="red darken-2" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong>{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                                <p class="small text-uppercase fw-bold">Vue JS </p>
                                <v-progress-linear v-model="vue" color="green" height="15" class="mb-5">
                                    <template v-slot:default="{ value }">
                                        <strong>{{ Math.ceil(value) }}%</strong>
                                    </template>
                                </v-progress-linear>
                                
                            </v-container>
                        </div>
                    </div>
                </div>
            </div>
        </v-container>
    </section>
</template>
<script>
export default {
    name: 'My-Noob-Skills',
    data: () => ({
        html: 95,
        css: 90,
        js: 40,
        laravel: 39,
        vue: 10,
        boot: 80,
        knowledge: 33,
        power: 78,
    }),
}
</script>