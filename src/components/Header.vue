<template>
  <div>
    <v-navigation-drawer v-model="drawer" app>
      <v-list dense>
        <v-list-item link @click="$vuetify.goTo(0)">
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>TOP</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="$vuetify.goTo(href='#about')">
          <v-list-item-action>
            <v-icon>mdi-account</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>ABOUT</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="$vuetify.goTo(href='#skills')">
          <v-list-item-action>
            <v-icon>mdi-pencil</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>SKILLS</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="$vuetify.goTo(href='#workes')">
          <v-list-item-action>
            <v-icon>mdi-widgets</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>WORKES</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-switch v-model="$vuetify.theme.dark" label="Dark"></v-switch>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar dense app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-btn text @click="$vuetify.goTo(0)">TOP</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#about')">ABOUT</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#skills')">SKILLS</v-btn>
      <v-btn text @click="$vuetify.goTo(href='#workes')">WORKES</v-btn>

      <v-spacer></v-spacer>
      <v-switch class="mt-5" v-model="$vuetify.theme.dark" label="Dark"></v-switch>
    </v-app-bar>
  </div>
</template>

<script>

  export default {
    data() {
      return {
        drawer: false,
      }
    },
  }
</script>