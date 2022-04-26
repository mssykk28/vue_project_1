<template>
  <v-app>
    <v-main>
      <WireFrame />
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import WireFrame from "./components/WireFrame.vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    //
  }),
  components: {
    WireFrame,
  },
});
</script>
