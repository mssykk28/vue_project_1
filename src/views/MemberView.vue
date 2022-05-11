<template>
  <v-expansion-panels>
    <v-expansion-panel v-for="item in items" :key="item.name">
      <v-expansion-panel-header> {{ item.name }} </v-expansion-panel-header>
      <v-expansion-panel-content>
        <v-container>
          <v-col class="px-5 py-5">
            <v-row no-gutters justify="center" align-content="center">
              <v-btn
                height="80"
                width="160"
                color="primary"
                elevation="0"
                class="mr-3"
              >
                稼働開始
              </v-btn>
              <v-btn height="80" width="160" color="error" elevation="0">
                稼働終了
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
              >
                休憩開始
              </v-btn>
              <v-btn height="80" width="160" outlined color="error">
                休憩終了
              </v-btn>
            </v-row>
          </v-col>
        </v-container>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>
<script lang="ts">
export default {
  data: () => ({
    items: [
      { name: "Name1" },
      { name: "Name2" },
      { name: "Name3" },
      { name: "Name4" },
    ],
  }),
};
</script>
<style></style>
