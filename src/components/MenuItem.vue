<template>
  <v-list-item>
    <v-list-item-title>
      <v-row class="ml-1">
        <v-col cols="3"
          ><v-icon><slot name="icon"></slot></v-icon
        ></v-col>
        <v-col cols="8" class="pt-4"><slot name="bodyText"></slot></v-col>
      </v-row>
    </v-list-item-title>
  </v-list-item>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "MenuItem",
  data() {
    return {};
  },
});
</script>
