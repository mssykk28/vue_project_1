<template>
  <v-app id="inspire">
    <header>
      <v-app-bar app dark>
        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
        <v-toolbar-title>MySuite</v-toolbar-title>
      </v-app-bar>
      <v-navigation-drawer v-model="drawer" fixed temporary>
        <v-list nav dense>
          <v-list-item-group>
            <MenuItem>
              <template v-slot:icon> mdi-home </template>
              <template v-slot:bodyText> Home </template>
            </MenuItem>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
    </header>

    <v-main>
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
import MenuItem from "@/components/MenuItem";
export default {
  data: () => ({
    drawer: false,
  }),
  components: { MenuItem },
};
</script>
