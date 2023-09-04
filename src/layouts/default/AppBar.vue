<template>
  <v-app-bar flat height="150">
    <v-app-bar-title>Stine og Marius</v-app-bar-title>
    <div class="music">
      <div v-if="musicPlaying" class="v-btn toggle-music" @click="stopMusic">
        <v-icon icon="mdi-music-note"></v-icon>
      </div>
      <div v-else class="v-btn toggle-music" @click="playMusic">
        <v-icon icon="mdi-music-note-off"></v-icon>
      </div>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppBar",
  data() {
    return {
      musicPlaying: false,
      music: new Audio(
        "https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Snow+Patrol+-+Chasing+Cars+-+Nick+Pitera+(cover).mp3"
      ),
    };
  },
  created() {
    this.music.addEventListener("ended", () => {
      this.musicPlaying = false;
      this.music.currentTime = 0;
    });
  },
  methods: {
    playMusic() {
      this.musicPlaying = true;
      this.music.play();
    },
    stopMusic() {
      this.musicPlaying = false;
      this.music.pause();
    },
  },
};
</script>

<style scoped>
header.v-app-bar {
  background-color: #b2ac88;
  color: #000000;
}

.music {
  position: fixed;
  right: 30px;
  top: 40px;
  margin: 1rem;
  font-size: 20px;
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

@font-face {
  font-family: "Wedding Bells";
  src: url("/public/fonts/Wedding Bells - TTF.ttf") format("truetype");
}

@font-face {
  font-family: "Dosis";
  src: url("/public/fonts/Dosis-Medium.ttf") format("truetype");
}

@font-face {
  font-family: "GreatVibes";
  src: url("/public/fonts/GreatVibes-Regular.ttf") format("truetype");
}

@font-face {
  font-family: "Alexis Marie";
  src: url("/public/fonts/Alexis Marie.ttf") format("truetype");
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
