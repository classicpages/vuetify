<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
      <v-btn icon>
        <v-icon color="#fff" icon>fas fa-dragon</v-icon>
      </v-btn>
  
      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')">Home</v-btn>
      <v-btn text @click="scroll('project')">Project</v-btn>
      <v-btn text @click="scroll('about')">about</v-btn>
      <v-btn text @click="scroll('contact')"> contact</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style scoped>
  .app{
    color: #fff;
    padding-left: 8px;
    padding-right: 8px;
  }
  .icon {
    color: white;
    background-color: #111111;
  }
  </style>