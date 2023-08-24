<template>
  <div class="full-width background-image">
    <v-container>
      <v-row>
        <v-col cols="12"> </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.background-image {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-006.jpg");
  background-color: #b2ac88;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: calc(~"100vh - 150px");
  width: 100vw;
  position: relative;
}
</style>
