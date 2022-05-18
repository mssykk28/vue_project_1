<template>
  <v-expansion-panels>
    <v-expansion-panel v-for="item in items" :key="item.name">
      <v-expansion-panel-header>
        {{ item.name }}
        <div class="ml-3">{{ condition }}</div>
      </v-expansion-panel-header>
      <v-expansion-panel-content :key="status">
        <v-container>
          <v-col class="px-5 py-5">
            <v-row no-gutters justify="center" align-content="center">
              <v-btn
                height="80"
                width="160"
                color="primary"
                elevation="0"
                class="mr-3"
                @click="showMessage(status.Name1)"
              >
                {{ status.Name1 }}
              </v-btn>
              <v-btn
                height="80"
                width="160"
                color="error"
                elevation="0"
                @click="showMessage(status.Name2)"
              >
                {{ status.Name2 }}
              </v-btn>
            </v-row>
          </v-col>
          <v-col class="px-5 py-5">
            <v-row no-gutters justify="center" align-content="center">
              <v-btn
                height="80"
                width="160"
                outlined
                color="primary"
                class="mr-3"
                @click="showMessage(status.Name3)"
              >
                {{ status.Name3 }}
              </v-btn>
              <v-btn
                height="80"
                width="160"
                outlined
                color="error"
                @click="showMessage(status.Name4)"
              >
                {{ status.Name4 }}
              </v-btn>
            </v-row>
          </v-col>
        </v-container>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>
<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    condition: "",
    dialog: false,
    items: [
      { name: "Name1" },
      { name: "Name2" },
      { name: "Name3" },
      { name: "Name4" },
    ],
    status: {
      Name1: "稼働開始",
      Name2: "稼働終了",
      Name3: "休憩開始",
      Name4: "休憩終了",
    },
  }),
  methods: {
    showMessage(condition: string) {
      this.condition = condition;
    },
  },
});
</script>
<style></style>
