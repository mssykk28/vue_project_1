<template>
  <header>
    <v-app-bar app dark>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>MySuite</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" fixed temporary>
      <v-list nav>
        <v-list-item-group>
          <v-list-item to="/home">
            <v-list-item-title>
              <v-row class="ml-1">
                <v-col cols="3"><v-icon>mdi-home</v-icon></v-col>
                <v-col cols="8" class="pt-4">Home </v-col>
              </v-row>
            </v-list-item-title>
          </v-list-item>

          <v-list-item to="/account">
            <v-list-item-title>
              <v-row class="ml-1">
                <v-col cols="3"><v-icon>mdi-account</v-icon></v-col>
                <v-col cols="8" class="pt-4">Account </v-col>
              </v-row>
            </v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </header>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
  }),
  components: {},
};
</script>
