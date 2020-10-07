<template>
  <v-container class="workes">
    <h1>WORKES</h1>
      <v-row justify="center" align="center" class="workes-item">
        <div class="mx-3">
          <modal1/>
        </div>
        <div class="mx-3">
          <modal2/>
        </div>
        <div class="mx-3">
          <modal3/>
        </div>
      </v-row>
  </v-container>
</template>

<script>
  import Modal1 from '../components/Modal1.vue';
  import Modal2 from '../components/Modal2.vue';
  import Modal3 from '../components/Modal3.vue';


  export default {
    components: {
      Modal1,
      Modal2,
      Modal3
    }
  }
</script>

<style>
  .workes-item {
    margin: 180px 0;
  }
</style>