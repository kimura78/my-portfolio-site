<template>
  <v-container class="skills mt-16 mb-16">
    <div class="skills-header mb-3">
      <h1>SKILLS</h1>
    </div>

      <v-row>
        <div class="mt-10 mx-16">
          <v-row>
            <i class="devicon-javascript-plain colored mr-5 mt-5"></i>
            <div class="skill-text">
              <h3>Javascript</h3>
              <p>基本的なことはわかるが、書いた量は多くない</p>
              <p>もっと勉強していきたい</p>
              <v-rating small readonly v-model="javascript"></v-rating>
            </div>
          </v-row>
        </div>

        <div class="vue mt-10 ml-16">
          <v-row>
            <i class="devicon-laravel-plain colored mr-5 mt-5"></i>
            <div class="skill-text">
              <h3>Laravel</h3>
              <p>最近使い始めた</p>
              <p>今後メインで使っていきたい</p>
              <v-rating small readonly v-model="html"></v-rating>
            </div>
          </v-row>
        </div>  
      </v-row>

      <v-row>
        <div class="ruby mt-10 mx-16">
          <v-row>
            <i class="devicon-rails-plain colored mr-5 mt-5"></i>
            <div class="skill-text mr-16">
              <h3>Ruby on Rails</h3>
              <p>最も長く触っているFW</p>
              <p>SNSサービスや予約システムを作った</p>
              <v-rating small readonly v-model="ruby"></v-rating>
            </div>
          </v-row>
        </div>

        <div class="vue mt-10 ml-16">
          <v-row>
            <i class="devicon-vuejs-plain colored mr-5 mt-5"></i>
            <div class="skill-text">
              <h3>Vue.js</h3>
              <p>このサイトを作った</p>
              <p>axiosを使った API + Vueが得意</p>
              <v-rating small readonly v-model="vue"></v-rating>
            </div>
          </v-row>
        </div>
      </v-row>

      <v-row>
        <div class="docker mt-10 mx-16">
          <v-row>
            <i class="devicon-docker-plain colored colored mr-5 mt-5"></i>
            <div class="skill-text mr-16">
              <h3>Docker</h3>
              <p>Dockerfileが書ける</p>
              <p>EC2 + Dockerで開発することが多い</p>
              <v-rating small readonly v-model="docker"></v-rating>
            </div>
          </v-row>
        </div>

        <div class="aws mt-10 ml-16">
          <v-row>
            <i class="devicon-amazonwebservices-plain colored mr-5 mt-5"></i>
            <div class="skill-text">
              <h3>AWS</h3>
              <p>EC2/RDS/S3/ACM/IAMなどは使える</p>
              <p>素早くEC2構築からDocker導入までできる</p>
              <v-rating small readonly v-model="aws"></v-rating>
            </div>
          </v-row>
        </div>
      </v-row>

  </v-container>
</template>

<script>
export default {
  data() {
    return {
      html: 3,
      javascript: 3,
      ruby: 4,
      vue: 4,
      docker: 4,
      aws: 4,
    }
  },
}
</script>

<style>
  .skills i {
    font-size: 6rem;
  }
</style>