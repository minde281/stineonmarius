<template>
  <div class="full-width background-image top-image">
    <div class="image-text bottom">
      <p class="date">22. juni 2024</p>
      <p class="sub-text">Bli med og feire dagen med oss</p>
    </div>
  </div>
  <div class="full-width the-day">
    <div class="center-text">
      <div class="time-table">
        <p class="header">Program</p>
        <v-row>
          <v-col class="text-rigth" cols="12" sm="6">
            <p class="display-1">12:00</p>
          </v-col>
          <v-col class="text-left" cols="12" sm="6">
            <p class="display-1">Puling i fjæra</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-rigth" cols="12" sm="6">
            <p class="display-1">14:00</p>
          </v-col>
          <v-col class="text-left" cols="12" sm="6">
            <p class="display-1">Analen i kanalen</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-rigth" cols="12" sm="6">
            <p class="display-1">16:00</p>
          </v-col>
          <v-col class="text-left" cols="12" sm="6">
            <p class="display-1">Snusken i busken</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-rigth" cols="12" sm="6">
            <p class="display-1">18:00</p>
          </v-col>
          <v-col class="text-left" cols="12" sm="6">
            <p class="display-1">BK</p>
          </v-col>
        </v-row>
      </div>
      <br />
      <br />
      <h1>Program</h1>
      <h3>Sermoni</h3>
      <h2>Rotvol park</h2>
      <h3>Selskap</h3>
      <h2>Scandic Nidelven</h2>
    </div>
  </div>
  <div class="full-width background-image image-stare">
    <div class="image-text top">
      <div class="timer">
        <vue-countdown :time="timer" v-slot="{ days, hours, minutes, seconds }">
          <div class="flex">
            <div title="Dager" class="days">
              <p>Dager</p>
              {{ days }}
            </div>
            <div title="Timer" class="hours">
              <p>Timer</p>
              {{ hours }}
            </div>
            <div title="Minutter" class="minutes">
              <p>Minutter</p>
              {{ minutes }}
            </div>
            <div title="Sekunder" class="seconds">
              <p>Sekunder</p>
              {{ seconds }}
            </div>
          </div>
        </vue-countdown>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({}),
  computed: {
    timer() {
      const now = new Date();
      const newYear = Date.parse("2024-06-22 14:00:00");

      return newYear - now;
    },
  },
};
</script>

<style lang="less" scoped>
@background-color: #ffffff;
@text-box-background-color: #b2ac88;
@text-box-text-color: #000000;
@default-font: "Alexis Marie", sans-serif;

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: @background-color;
}

.background-image {
  background-color: @background-color;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.full-width {
  height: calc(~"100vh - 150px");
  width: 100vw;
  max-width: 1920px;
  position: relative;
  background-color: @text-box-background-color;
}

.image-text {
  position: absolute;
  width: 75vh;
  left: 50%;
  transform: translate(-50%, 0);
  color: @text-box-text-color;
  font-family: @default-font;
  font-weight: 100;
  text-align: center;
  overflow: visible;
  height: auto;
  background-color: @text-box-background-color;

  &.bottom {
    bottom: 0%;
    border-radius: 20px 20px 0 0;
    padding: 40px 80px 20px 80px;
    p {
      font-size: 30px;
      &.date {
        font-size: 50px;
      }
    }
  }
  &.top {
    top: 0%;
    border-radius: 0 0 20px 20px;
    padding: 20px 80px 40px 80px;
  }
}

.center-text {
  position: absolute;
  width: 75vh;
  top: 0%;
  bottom: 0%;
  left: 50%;
  transform: translate(-50%, 0);
  color: @text-box-text-color;
  font-family: @default-font;
  font-weight: 100;
  text-align: center;
  overflow: visible;
  height: auto;
  background-color: @text-box-background-color;
}

.top-image {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-006.jpg");
}

.image-stare {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-001-bw.jpg");
}

.timer {
  padding-top: 20px;
  display: block;
  text-align: center;
  font-family: "LoversQuarrel", sans-serif;
  overflow: visible;
  height: auto;
  div {
    font-size: 50px;
    padding: 0 30px;
    p {
      font-size: 40px;
      font-family: "Andasia", sans-serif;
      text-align: center;
      overflow: visible;
      height: auto;
    }
  }
}

.time-table {
  font-size: 40px;
  .header {
    font-size: 60px;
    font-family: "Andasia", sans-serif;
    text-align: center;
    overflow: visible;
    height: auto;
  }
}

.text-rigth {
  text-align: right;
}

.text-left {
  text-align: left;
}

.flex {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
</style>
