<template>
  <v-dialog v-model="dialog" max-width="800">
    <template v-slot:activator="{ on, attrs }">
      <img class="elevation-5" v-bind="attrs" v-on="on" src="../assets/heyatori.png" height="180px"/>
    </template>

    <v-card class="mx-auto">
      <v-col cols="auto">
        <v-img class="elevation-5" src="../assets/heyatori.png"></v-img>
      </v-col>

      <v-card-subtitle class="pb-0">部屋取りアプリ</v-card-subtitle>
      <v-card-text class="text--primary">
        <div>Rails API + Vue.jsで作成した部屋予約アプリです。</div>

        <div>オンライン上で作成した部屋をグループ内のユーザーが予約できるアプリです。</div>

        <a href="https://www.heyatori-app.tk" target="_blank" >https://www.heyatori-app.tk</a>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn text @click="dialog = false">Close</v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>

<script>
  export default {
    data() {
      return {
        dialog: false,
      }
    },
  }
</script>

<style>
</style>