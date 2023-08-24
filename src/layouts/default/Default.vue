<template>
  <v-app>
    <div class="container">
      <default-bar />

      <default-view />
    </div>
  </v-app>
</template>

<script setup>
import DefaultBar from "./AppBar.vue";
import DefaultView from "./View.vue";
</script>

<style lang="less" scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #6b6b6b;
}
</style>
