<template>
  <v-app>
    <Header/>
    <v-main>
      <Top id="top"/>
      <About id="about"/>
      <Skills id="skills"/>
      <Workes id="workes"/>
    </v-main>
  </v-app>
</template>

<script>
  import Header from './components/Header.vue';
  import Top from './components/Top.vue';
  import About from './components/About.vue'; 
  import Skills from './components/Skills.vue';
  import Workes from './components/Workes.vue';

  export default {
    name: 'App',

    components: {
      Header,
      Top,
      About,
      Skills,
      Workes,
    },
  };
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Recursive:wght@300&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=M+PLUS+1p:wght@300&display=swap');
  
  #app {
    font-family: 'Recursive', 'M PLUS 1p', sans-serif;
  }
  i {
    font-size: 1.7rem;
  }
</style>
