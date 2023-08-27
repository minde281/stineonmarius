<template>
  <v-app-bar flat height="150">
    <v-app-bar-title>Stine og Marius</v-app-bar-title>
  </v-app-bar>
</template>

<script></script>

<style scoped>
header.v-app-bar {
  background-color: #ffffff;
  color: #000000;
}
</style>

<style lang="less">
@font-face {
  font-family: "I Love Glitter";
  src: url("/public/fonts/I Love Glitter.ttf") format("truetype");
}

@font-face {
  font-family: "Monsieur-Regular";
  src: url("/public/fonts/MonsieurLaDoulaise-Regular.ttf") format("truetype");
}

@font-face {
  font-family: "The heart of everything";
  src: url("/public/fonts/The Heart of Everything - TTF.ttf") format("truetype"),
    url("/public/fonts/The Heart of Everything - OTF.otf") format("otf");
}

@font-face {
  font-family: "Brotherhood";
  src: url("/public/fonts/Brotherhood_Script.ttf") format("truetype");
}

@font-face {
  font-family: "Andasia";
  src: url("/public/fonts/Andasia.ttf") format("truetype");
}

@font-face {
  font-family: "LoversQuarrel";
  src: url("/public/fonts/LoversQuarrel-Regular.ttf") format("truetype");
}

@font-face {
  font-family: "Mrs Alexandra";
  src: url("/public/fonts/Mrs Alexandra.ttf") format("truetype");
}

.v-toolbar__content {
  .v-toolbar-title__placeholder {
    font-family: "Andasia", sans-serif;
    font-size: 5rem;
    font-weight: 100;
    text-align: center;
    overflow: visible;
    height: auto;
  }
}
</style>
