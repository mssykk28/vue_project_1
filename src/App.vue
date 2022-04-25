<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <VuetifyLogo />
        <VuetifyName />
      </div>

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import VuetifyLogo from "./components/VuetifyLogo.vue";
import VuetifyName from "./components/VuetifyName.vue";

export default Vue.extend({
  name: "App",

  data: () => ({
    //
  }),
  components: {
    VuetifyLogo,
    VuetifyName,
  },
});
</script>
