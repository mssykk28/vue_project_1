<template>
  <v-app>
    <WireFrame />
    <v-main>
      <router-view></router-view>
    </v-main>
    <template>
      <v-footer dark padless>
        <v-row justify="center" no-gutters>
          <v-btn
            v-for="link in links"
            :key="link"
            color="white"
            text
            rounded
            class="my-2"
          >
            {{ link }}
          </v-btn>
          <v-col class="py-4 text-center white--text" cols="12">
            {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
          </v-col>
        </v-row>
      </v-footer>
    </template>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";

import WireFrame from "@/components/WireFrame.vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    links: ["Home", "About Us", "Team", "Services", "Blog", "Contact Us"],
  }),
  components: {
    WireFrame,
  },
});
</script>
<style></style>
