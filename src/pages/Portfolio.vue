<template>
  <v-app-bar>
    <v-app-bar-nav-icon>
      <v-spacer />

      <v-menu>
        <template #activator="{ props }">
          <v-app-bar-nav-icon variant="text" v-bind="props" />
        </template><v-list>
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            :value="i"
          >
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list></v-menu></v-app-bar-nav-icon>
    <v-app-bar-title>Home</v-app-bar-title>
    <v-btn class="cursor-pointer" to="About">About</v-btn>
    <v-btn
      class="mr-5 cursor-pointer"
      color="teal-darken-2"
      href="mailto:yogesh628882@gmail.com"
      icon="mdi-email"
      size="large"
      target="_blank"
    />
    <v-btn
      color="primary"
      href="https://github.com/Yogesh18707"
      rounded="lg"
      size="small"
      target="_blank"
      variant="outlined"
    > Github</v-btn>
  </v-app-bar>
  <v-card-item>
    <div class="d-flex justify-center w-100 h-100">
      <img class="rounded-circle" height="200" src="../assets/WhatsApp Image 2025-07-08 at 11.14.35_01b5ff42.jpg" width="200">
      <span><v-card class="text-center rounded-t bg-shades-white elevation-24" width="170">
        <v-card-title>
          Hi, I'm Yogesh
        </v-card-title>
        <v-card-subtitle><v-icon><img height="15" src="../assets/office.png" width="15"></v-icon> Front End Developer</v-card-subtitle>
      </v-card></span>
    </div></v-card-item>
  <div class="d-flex justify-center">
    <v-container class="d-inline-flex justify-center bg-amber rounded-xl justify-space-around ">
      <v-btn class="bg-transparent" color="white" href="#Skills">Skills</v-btn>
      <v-btn class="bg-transparent" color="white" :to="{path: '/about', hash:'#Education' }">Education</v-btn>
      <v-btn class="bg-transparent" color="white" href="#Projects">Projects</v-btn>
    </v-container>
  </div>
  <v-container class="d-flex justify-center flex-column">
    <h1 id="Skills">Skills</h1>
    <hr>
    <div class="d-flex justify-space-evenly">
      <v-btn class="rounded-xl mt-5" color="white">HTMl</v-btn>
      <v-btn class="rounded-xl mt-5" color="white">CSS</v-btn>
      <v-btn class="rounded-xl mt-5" color="white">JAVA SCRIPT</v-btn>
      <v-btn class="rounded-xl mt-5" color="white">VUE</v-btn>
      <v-btn class="rounded-xl mt-5" color="white"><v-hover style="background-color: white">VUETIFY</v-hover></v-btn>
    </div>
  </v-container>
  <v-container class="d-flex justify-center flex-column mt-16">
    <h1 id="Projects">Projects</h1>
    <v-card-subtitle>To view projects click on the GitHub button</v-card-subtitle>
    <hr>
    <div class="d-flex justify-space-evenly">
      <v-btn class="rounded-xl mt-5" color="white">To-Do App</v-btn>
      <v-btn class="rounded-xl mt-5" color="white">Portfolio</v-btn>

    </div>
  </v-container>
  <v-footer class="d-flex flex-column  align-start mt-16">
    <v-card-subtitle>&copy; 2025 Yogesh. All Right Reserved</v-card-subtitle>

    <v-card-title>
      Contact Options:
    </v-card-title>
    <v-card-item>
      <v-card-title class="d-flex align-center ga-5"><img height="30" src="../assets/call.webp" width="30"><a :href="`tel:${8295839288}`">{{ 8295836288 }}</a></v-card-title>
      <v-card-title class="d-flex align-center ga-5"><v-icon icon="mdi-email" /><a href="mailto:yogesh628882@gmail.com">yogesh628882@gmail.com</a></v-card-title>
      <v-card-title class="d-flex align-center ga-5"><img height="30" src="../assets/1731430269_logo-instagram-png.png" width="30"><a href="https://www.instagram.com/its_sandybasduda">its_sandybasduda</a></v-card-title>

    </v-card-item>
  </v-footer>

</template>

<script lang="ts" setup>
  interface Faces {
    title: string
    About: any
  }
  const items = [
    { title: 'Home' },
    { title: 'About' },
    { title: 'Education' },
    { title: 'Projects' },
  ]
</script>

<style scoped>
a{
  text-decoration: none;
  color: white;
}

</style>
