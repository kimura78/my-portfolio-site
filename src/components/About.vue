<template>
  <v-container class="mt-16 mb-15">
    <h1>About</h1>
    <p>MASANORI KIMURA</p>
    <v-col class="text-center">

      <div>
        <img src="../assets/profile.png" height="150px">
        <p></p>
        <p>主にRuby on Rails・Vue.jsを使って開発をしています</p>
        <p>現在転職活動中です</p>
        <v-btn text href="https://github.com/kimura78" class="mt-3">
          <i class="devicon-github-plain-wordmark"></i>
        </v-btn>
      </div>    
      <v-timeline>
        <v-timeline-item
          v-for="(year, i)  in years"
          :key="i"
          large
          :color="year.color">
          
          <template v-slot:opposite>
            <span
              :class="`headline ${year.color}--text`"
              v-text="year.year"
            ></span>
          </template>
          
          <div class="py-12">
            <v-card class="elevation-2 rounded-pill">
              <v-card-text v-text="year.text" bold></v-card-text>
            </v-card>
          </div>

        </v-timeline-item>
      </v-timeline>
    </v-col>

  </v-container>
</template>

<script>
  export default {
    data() {
      return {
        years: [
        {
          color: 'indigo',
          year: '1997',
          text: '1997年生まれ 埼玉県在住',
        },
        {
          color: 'teal',
          year: '2019',
          text: 'プログラミングに初めて触る',
        },
        {
          color: 'blue',
          year: '2020',
          text: '2020年3月 獨協大学卒業'
        },
      ],
      }
    },
  }
</script>

<style>
</style>