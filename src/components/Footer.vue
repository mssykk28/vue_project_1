<template>
  <v-footer dark padless>
    <v-row justify="center" no-gutters>
      <v-btn to="/" class="my-2" color="white" text>Home</v-btn>
      <v-btn to="/account" class="my-2" color="white" text>Account</v-btn>
      <v-btn to="/calendar" class="my-2" color="white" text>Calendar</v-btn>
      <v-col class="py-4 text-center white--text" cols="12">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>
<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    links: [
      { name: "Home", path: "/" },
      { name: "Account", path: "/account" },
      { name: "Calendar", path: "/calendar" },
    ],
  }),
  components: {},
});
</script>
<style></style>
