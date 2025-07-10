<template>
  <v-app-bar>
    <v-app-bar-nav-icon>
      <v-spacer />

      <v-menu
        offset-y
        open-on-hover
        transition="scale-transition"
      >
        <template #activator="{ props }">
          <v-app-bar-nav-icon variant="text" v-bind="props" />
        </template><v-list>
          <v-list-item to="/">Home</v-list-item>
          <v-list-item to="/about">About</v-list-item>
        </v-list></v-menu></v-app-bar-nav-icon>
    <v-btn
      icon
      @click="goback()"
    >
      <v-icon icon="mdi-arrow-left" />
    </v-btn>
    <v-app-bar-title>About</v-app-bar-title>

    <v-btn
      class="mr-5 cursor-pointer"
      color="teal-darken-2"
      href="mailto:yogesh628882@gmail.com"
      icon="mdi-email"
      size="large"
      target="_blank"
    />
    <v-btn href="https://github.com/Yogesh18707" rounded="lg" size="small" variant="outlined" class="github"> Github</v-btn>
  </v-app-bar>
  <v-card class="pa-4 text-center justify-center" color="white">
    <v-card-title>Skills</v-card-title>
    <v-card-text>
      I'm a front-end web developer specializing in building modern, responsive, and high-performance user interfaces using HTML, CSS, JavaScript, and Vue.js with TypeScript. With a strong foundation in web standards and component-based architecture, I craft clean, maintainable code and scalable front-end solutions. My focus is on delivering seamless user experiences through efficient design systems and interactive features powered by Vue's reactive core.
    </v-card-text>
  </v-card>
  <v-card-item>
    <div class="d-flex justify-space-evenly">
      <v-img
        height="100"
        src="../assets/3d-html-icon-symbols-of-software-language-png.webp"
        width="100"
      />
      <v-img
        height="100"
        src="../assets/pngtree-coding-language-css-system-vector-isometric-sign-png-image_4687821.png"
        width="100"
      /></div>
    <div class="d-flex justify-space-evenly mt-5">
      <v-img
        height="100"
        src="../assets/7578002.webp"
        width="100"
      />
      <v-img
        height="100"
        src="../assets/3640297.webp"
        width="100"
      />
    </div>
  </v-card-item>
  <v-card class="text-center">
    <v-card-title>
      About
    </v-card-title>
    <v-card-text class="elevation-24">
      I'm Yogesh, a passionate and detail-oriented Frontend Developer from Basduda village, Rewari district, Haryana. I specialize in building responsive, user-friendly web interfaces using modern technologies like HTML, CSS, JavaScript, and React. Committed to writing clean, efficient code and continuously learning to stay updated in the fast-evolving tech landscape.
    </v-card-text>
  </v-card>
  <hr>
  <v-card class="mt-5">
    <v-card-title>
      <h1 id="Education" class="text-green-darken-2"> <b>Educations </b></h1>
    </v-card-title>
    <v-list>
      <v-list-item>
        <h1> • ITI (COPA Trade)</h1>
        <v-card-title>Completed Computer Operator and<br> Programming Assistant (COPA) trade <br>from Industrial Training Institute (ITI).</v-card-title>
      </v-list-item>
      <v-list-item>
        <h1> • 12th Standard</h1>
        <v-card-title>Passed 12th from Aastha Public School <br> under HBSE(Haryana Board of School<br> Education) with 68.4% marks.</v-card-title>
      </v-list-item>
      <v-list-item>
        <h1> • 10th Standard</h1>
        <v-card-title>Passed 10th from Vivekanand Sr. Sec.<br>  School under CBSE (Central Board of <br> Secondary Education) with a 9.4 CGPA.</v-card-title>
      </v-list-item>
    </v-list>
  </v-card>
  <v-card class="d-flex justify-center">
    <img
      height="100"
      src="../assets/thank-you-visiting-us-vector-260nw-1214737042.webp"
      width="700"
    >
  </v-card>
  <v-footer class="d-flex flex-column  justify-start mt-5 align-start mt-16">
    <v-card-subtitle>&copy; 2025 Yogesh. All Right Reserved</v-card-subtitle>
    <h2>Contact Options:</h2>
    <v-card-item>
      <v-card-title class="d-flex align-center ga-5"><img height="30" src="../assets/call.webp" width="30"><a :href="`tel:${8295839288}`">{{ 8295836288 }}</a></v-card-title>
      <v-card-title class="d-flex align-center ga-5"><v-icon icon="mdi-email" /><a href="mailto:yogesh628882@gmail.com">yogesh628882@gmail.com</a></v-card-title>
      <v-card-title class="d-flex align-center ga-5"><img height="30" src="../assets/1731430269_logo-instagram-png.png" width="30"><a href="https://www.instagram.com/its_sandybasduda">its_sandybasduda</a>
      </v-card-title>
    </v-card-item>
  </v-footer>
</template>
<script setup lang="ts">
  function goback() {
 window.history.back()  }
</script>
<style scoped>
a{
  text-decoration: none;
  color: white;
}
.github:hover{
  background-color: darkred;
  color: white;
}

</style>
