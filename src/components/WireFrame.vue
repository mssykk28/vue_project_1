<template>
  <header>
    <v-app-bar app dark>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>MySuite</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" fixed temporary>
      <v-list nav>
        <v-list-item-group>
          <v-list-item to="/">
            <v-list-item-title>
              <v-row class="ml-1">
                <v-col cols="3"><v-icon>mdi-home</v-icon></v-col>
                <v-col cols="8" class="pt-4">Home </v-col>
              </v-row>
            </v-list-item-title>
          </v-list-item>

          <v-list-item to="/members">
            <v-list-item-title>
              <v-row class="ml-1">
                <v-col cols="3"><v-icon>mdi-account-group</v-icon></v-col>
                <v-col cols="8" class="pt-4">Members </v-col>
              </v-row>
            </v-list-item-title>
          </v-list-item>

          <v-list-item to="/calendar">
            <v-list-item-title>
              <v-row class="ml-1">
                <v-col cols="3"><v-icon>mdi-calendar</v-icon></v-col>
                <v-col cols="8" class="pt-4">Calendar </v-col>
              </v-row>
            </v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </header>
</template>

<script lang="ts">
export default {
  data: () => ({
    drawer: false,
  }),
  components: {},
};
</script>
