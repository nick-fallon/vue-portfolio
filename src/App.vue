<template>
  <div id="app">
    <v-app>
      <v-navigation-drawer absolute persistent light v-model="drawer" overflow>
        <v-toolbar flat>
          <v-list class="pa-0">
            <v-list-tile avatar>
              <v-list-tile-avatar>
                <img src="https://randomuser.me/api/portraits/men/85.jpg" />
              </v-list-tile-avatar>
              <v-list-tile-content>
                <v-list-tile-title>Nick Fallon</v-list-tile-title>
              </v-list-tile-content>
            </v-list-tile>
          </v-list>
        </v-toolbar>
        <v-list class="pt-0" dense>
          <v-divider></v-divider>
          <v-list-tile v-for="item in items" :key="item.title" @click="" :href="item.route">
            <v-list-tile-action>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>{{ item.title }}</v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
        </v-list>
      </v-navigation-drawer>
      <v-toolbar fixed class="cyan darken-4" dark>
        <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
        <v-toolbar-title>Nick Fallon</v-toolbar-title>
      </v-toolbar>
      <main>
        <v-container fluid>
          <router-view></router-view>
        </v-container>
      </main>
    </v-app>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
      return {
        drawer: true,
        items: [
          { title: 'Home', icon: 'fa-home', route: '/' },
          { title: 'About', icon: 'fa-question', route: '/#/about' },
          { title: 'Projects', icon: 'fa-flask' , route: '/#/projects'},
          { title: 'Contact Me', icon: 'fa-comment-o', route: '/#/contact' }
        ],
        right: null
      }
    }
}
</script>

<style>
body {
  margin: 0;
  font-family: 'Josefin Sans', Helvetica, sans-serif;
}
.container {
  padding: 0;
}

</style>
