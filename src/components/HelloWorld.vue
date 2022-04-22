<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <template>
        <v-card class="mx-auto" max-width="300" tile>
          <v-list flat>
            <v-subheader>Tab</v-subheader>
            <v-list-item-group v-model="selectedItem" color="primary">
              <v-list-item v-for="(item, i) in items" :key="i">
                <v-list-item-icon>
                  <v-icon v-text="item.icon"></v-icon>
                </v-list-item-icon>
                <v-list-item-content>
                  <v-list-item-title v-text="item.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card>
      </template>
    </v-navigation-drawer>

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
export default {
  data: () => ({
    drawer: null,
    selectedItem: 1,
    items: [
      { text: "Account", icon: "mdi-account" },
      { text: "Test0", icon: "mdi-flag" },
      { text: "Test1", icon: "mdi-flag" },
      { text: "Test2", icon: "mdi-flag" },
      { text: "Test3", icon: "mdi-flag" },
      { text: "Test4", icon: "mdi-flag" },
      { text: "Test5", icon: "mdi-flag" },
      { text: "Test6", icon: "mdi-flag" },
    ],
  }),
};
</script>
