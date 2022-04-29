<template>
  <header>
    <v-app-bar app dark>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>MySuite</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" fixed temporary>
      <v-list nav>
        <v-list-item-group>
          <MenuItem>
            <template v-slot:icon> mdi-home </template>
            <template v-slot:bodyText> Home </template>
          </MenuItem>

          <MenuItem>
            <template v-slot:icon> mdi-account </template>
            <template v-slot:bodyText> Account </template>
          </MenuItem>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </header>
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
