<template>
  <v-card class="mx-auto" max-width="300" tile>
    <v-list flat>
      <v-subheader>Tab</v-subheader>
      <v-list-item-group v-model="selectedItem" color="primary">
        <v-list-item v-for="(item, i) in items" :key="i" :to="item.link">
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

<script>
export default {
  data: () => ({
    selectedItem: 1,
    items: [
      { text: "Account", icon: "mdi-account", link: "/account" },
      { text: "Test0", icon: "mdi-flag", link: "/test0" },
      { text: "Test1", icon: "mdi-flag", link: "/test1" },
      { text: "Test2", icon: "mdi-flag", link: "/test2" },
      { text: "Test3", icon: "mdi-flag", link: "/test3" },
      { text: "Test4", icon: "mdi-flag", link: "/test4" },
      { text: "Test5", icon: "mdi-flag", link: "/test5" },
      { text: "Test6", icon: "mdi-flag", link: "/test6" },
    ],
  }),
};
</script>
