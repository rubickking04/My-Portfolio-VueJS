<template>
  <section id="home">
    <v-container>
      <div class="py-5">
        <div class="py-5">
          <div class="py-5">
            <v-row class="text-center py-5">
              <div class="mb-4 col-lg-6 col-md-8">
                <div class="py-5">
                  <div class="py-5">
                    <div class="py-3 container">
                      <h5 class="headline px-2 text-start font-weight-bold">Hello, I'm </h5>
                      <h1 class="my-text display-3  text-start font-weight-bold my-name" style="font-family: 'Montserrat', sans-serif">{{ me }}</h1>
                      <p class="headline text-start font-weight-bold typing-text">I'm a Student Fullstack Developer.</p>
                      <div class="text-start mb-3">
                        <v-hover >
                          <a href="https://twitter.com/rubickking04"><span class="fs-1 bi bi-twitter text-secondary px-3"></span></a>
                        </v-hover>
                        <a href="https://www.facebook.com/alfhaigar.usman.1/" ><span class="fs-1 px-3 bi bi-facebook text-secondary"></span></a>
                        <a href="https://github.com/rubickking04"><span class="fs-1 px-3 bi bi-github text-secondary"></span></a>
                        <a href="https://www.instagram.com/kingrubick_04/"><span class="fs-1 bi bi-instagram text-secondary px-3"></span></a>
                        <a href="https://www.linkedin.com/in/al-fhaigar-usman-108812193/"><span class="fs-1 bi bi-linkedin text-secondary px-3"></span></a>
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
      </div>
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
h1 .my-name {
  font-family: "Montserrat", sans-serif;
}
.typing-text{
  margin-left: 10px;
  overflow: hidden;
  white-space: nowrap;
  border-right: 4px solid #1de2d1;
  animation: typing 5s  infinite;
}
@keyframes typing{
  0%{
    width: 0ch;
  }
  50%{
    width: 27ch;
  }
  100%{
    width: 0ch;
  }
}
/* @media (max-width: 400px) {
    h1 .my-text{
      font-size: 100px;
    }
  } */
</style>
