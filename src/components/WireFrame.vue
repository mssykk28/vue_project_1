<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <MenuItem
    /></v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
      <v-img
        :src="require('../assets/logo.svg')"
        class="my-3"
        contain
        height="200"
      />
    </v-main>
  </v-app>
</template>

<script>
import MenuItem from "./MenuItem";

export default {
  data: () => ({
    drawer: null,
  }),
  components: {
    MenuItem,
  },
};
</script>
