<template>
  <v-container class="mt-16 mb-15">
    <h1>About</h1>
    <p>MASANORI KIMURA</p>
    <v-col class="text-center">
      <v-timeline>
        <v-timeline-item
          v-for="(year, i)  in years"
          :key="i"
          large
          :color="year.color">
          
          <template v-slot:icon>
            <v-avatar>
              <img src="../assets/profile.png">
            </v-avatar>
          </template>

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
          text: '2020年3月 大学卒業後 転職活動中'
        },
      ],
      }
    },
  }
</script>

<style>
</style>