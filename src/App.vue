<template>
  <v-app>
    <Header/>
    <v-main>
      <Top/>
    </v-main>
  </v-app>
</template>

<script>
  import Header from './components/Header.vue';
  import Top from './components/Top.vue';

  export default {
    name: 'App',

    components: {
      Header,
      Top
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
