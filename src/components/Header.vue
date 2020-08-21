<template>
  <div>
    <v-navigation-drawer v-model="drawer" app>
      <v-list dense>
        <v-list-item link v-for="menu in menus" :key="menu.title" :to="menu.url">
          <v-list-item-action>
            <v-icon>{{ menu.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{ menu.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <i class="devicon-github-plain-wordmark"></i>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>GitHub</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-switch v-model="$vuetify.theme.dark" label="Dark"></v-switch>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar dense app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-btn text v-model="drawer" @click="$vuetify.goTo(0)">TOP</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#about')">ABOUT</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#skills')">SKILLS</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#workes')">WORKES</v-btn>

      <v-spacer></v-spacer>
      <v-btn text href="https://github.com/kimura78">
        <i class="devicon-github-plain-wordmark"></i>
      </v-btn>

      <v-switch class="mt-5" v-model="$vuetify.theme.dark" label="Dark"></v-switch>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menus: [
        { title: 'Top', icon: 'mdi-home', },
        { title: 'ABOUT', icon: 'mdi-account', },
        { title: 'SKILLS', icon: 'mdi-pencil', },
        { title: 'WORKES', icon: 'mdi-widgets', },
      ],
      drawer: false,
    }
  },
}
</script>