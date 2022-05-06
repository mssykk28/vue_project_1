<template>
  <v-expansion-panels>
    <v-expansion-panel v-for="(item, i) in 5" :key="i">
      <v-expansion-panel-header> Item </v-expansion-panel-header>
      <v-expansion-panel-content>
        <v-row align="center" justify="space-around">
          <v-btn color="primary"> 稼働開始 </v-btn>
          <v-btn color="error"> 稼働終了 </v-btn>
        </v-row>
        <v-row align="center" justify="space-around">
          <v-btn color="primary"> 休憩開始 </v-btn>
          <v-btn color="error"> 休憩終了 </v-btn>
        </v-row>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>
<script></script>
<style></style>
