<template>
  <v-app>
    <WireFrame />
    <v-main>
      <router-view></router-view>
    </v-main>
    <Footer />
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";

import WireFrame from "@/components/WireFrame.vue";
import Footer from "@/components/Footer.vue";

export default Vue.extend({
  name: "App",

  data: () => ({}),
  components: {
    WireFrame,
    Footer,
  },
});
</script>
<style></style>
