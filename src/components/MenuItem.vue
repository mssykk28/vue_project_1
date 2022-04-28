<template>
  <v-list-item>
    <v-list-item-title>
      <v-row>
        <v-col clos="2"
          ><v-icon><slot name="icon"></slot></v-icon
        ></v-col>
        <v-col clos="8"><slot name="bodyText"></slot></v-col>
      </v-row>
    </v-list-item-title>
  </v-list-item>
</template>

<script>
import Vue from "vue";
export default Vue.extend({
  name: "MenuItem",
  data() {
    return {};
  },
});
</script>
