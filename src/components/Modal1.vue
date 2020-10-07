<template>
  <v-dialog v-model="dialog" width="800">
    <template v-slot:activator="{ on, attrs }">
      <img class="elevation-5" v-bind="attrs" v-on="on" src="../assets/rchannel.png" height="180px"/>
    </template>

    <v-card class="mx-auto">
      <v-col cols="auto">
        <v-img class="elevation-5" src="../assets/rchannel.png"></v-img>
      </v-col>

      <v-card-subtitle class="pb-0">Rちゃんねる</v-card-subtitle>
      <v-card-text class="text--primary">
        <div>Ruby on Railsを使って初めて作成した記事投稿型のSNSサービスです。</div>

        <div>コメント機能(Ajax)や記事のカテゴリー分けが可能です。</div>

        <p>現在は公開していません。</p>
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