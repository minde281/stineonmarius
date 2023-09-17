<template>
  <div class="full-width background-image top-image">
    <div class="image-text bottom">
      <p class="big date">22. juni 2024</p>
      <p class="sub-text">Bli med og feire dagen med oss</p>
    </div>
  </div>
  <div class="full-width dynamic-height addresses">
    <div class="content">
      <div class="center-text">
        <div class="section sermoni">
          <p class="header">Sermoni</p>
          <p>Rotvoll Park</p>
          <p>Arkitekt Ebbells veg 22</p>
          <p>7053 Ranheim</p>
          <p>Bygg D, kl 14.00</p>
          <p></p>
          <br />
          <p>Etter sermonien blir det servert bobler og kake.</p>
          <p>De som ønsker kan være på Rotvoll Park frem til kl 16.00</p>
        </div>
        <div class="section">
          <p class="header">Selskap</p>
          <p>Scandic Nidelven</p>
          <p>Havnegata 1-3</p>
          <p>7010 Trondheim</p>
          <p>Kl 17.00</p>
          <p></p>
          <br />
          <p>Det servetes aperitiff,</p>
          <p>3-retters middag med drikke og kaffe.</p>
          <p>Ønskes noe utover dette kan det kjøpes i baren.</p>
        </div>
        <div class="section overnatting">
          <p class="header">Overnatting TODO</p>
          <p>
            Ønsker dere å overnatte på hotellet kan dere bruke rabattkode
            "RABATTKODE" ved bestilling.
          </p>
          <p>Da er Norges beste hotellfrokost inkludert.</p>
        </div>
        <div class="section kleskode">
          <p class="header">Kleskode</p>
          <p>
            Kleskoden er dress. Kle deg i noe du føler deg fin i og som du kan
            danse i.
          </p>
        </div>
        <div class="section toastmaster">
          <p class="header">Toastmaster TODO</p>
          <p>Vi har gleden av å presentere vår toastmaster</p>
          <p>Stine Minde</p>
          <br />
          <p>
            Dersom du har noe du ønsker å fortelle felleskapet ber vi deg varsle
            vår toastmaster på 81549300.
          </p>
          <p>Vi vil likevel be dere holde taler korte og underholdende</p>
        </div>
        <div class="section onskeliste">
          <p class="header">Gaver</p>
          <p>Vi er heldige og har alt vi trenger av materielle ting.</p>
          <p>Det vi skulle hatt mer av er tid sammen.</p>
          <p>Vi ønsker oss derfor et bidrag til bryllupsreise.</p>
        </div>
        <div class="section music">
          <p class="header">Musikk</p>
          <p>
            Hjelp oss gjerne med å lage spilleliste for kvelden. Har du en sang
            du vil høre kan du legge den til på
            <a
              target="_blank"
              href="https://open.spotify.com/playlist/2gmiGRcHdP1dnw4x6q5pvE?si=9a1503f03c6c4f96"
              >spotifylista vår</a
            >.
          </p>
        </div>
        <div class="section rsvp">
          <p class="header">Rsvp</p>
          <p>Gi gjerne beskjed om dere kommer eller ikke innen 15. april.</p>
          <p>Tlf Stine: 47898727</p>
          <p>Tlf Marius: 98401479</p>
        </div>
        <div class="section forlovere">
          <p class="header">Forlovere TODO</p>
          <div class="flex">
            <div class="forlover">
              <p>Stine</p>
              <p>Minde</p>
            </div>
            <div class="forlover">
              <p>Marius</p>
              <p>Minde</p>
            </div>
          </div>
        </div>
        <div class="section foto">
          <p class="header">Bilder</p>
          <p>
            Vi ønsker å samle alle bilder fra dagen. Har du tatt noen bilder kan
            du laste de opp
            <a
              target="_blank"
              href="https://photos.app.goo.gl/kpox96iZmP6dMSwB7"
              >her</a
            >.
          </p>
        </div>
      </div>
    </div>
  </div>
  <div class="full-width background-image image-stare"></div>
  <div class="full-width the-day">
    <div class="center-text">
      <div class="time-table">
        <p class="header">Program</p>
        <v-row>
          <v-col class="text-right" cols="6" sm="6">
            <p class="display-1">6:00</p>
          </v-col>
          <v-col class="text-left" cols="6" sm="6">
            <p class="display-1">Puling i fjæra</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-right" cols="6" sm="6">
            <p class="display-1">14:00</p>
          </v-col>
          <v-col class="text-left" cols="6" sm="6">
            <p class="display-1">Analen i kanalen</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-right" cols="6" sm="6">
            <p class="display-1">16:00</p>
          </v-col>
          <v-col class="text-left" cols="6" sm="6">
            <p class="display-1">Snusken i busken</p>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="text-right" cols="6" sm="6">
            <p class="display-1">18:00</p>
          </v-col>
          <v-col class="text-left" cols="6" sm="6">
            <p class="display-1">BK</p>
          </v-col>
        </v-row>
      </div>
    </div>
  </div>
  <div class="full-width background-image image-stare">
    <div class="image-text top">
      <div class="timer">
        <vue-countdown :time="timer" v-slot="{ days, hours, minutes, seconds }">
          <div class="flex">
            <div title="Dager" class="days">
              <p>Dager</p>
              <span class="mobile-only">D</span>
              {{ days }}
            </div>
            <div title="Timer" class="hours">
              <p>Timer</p>
              <span class="mobile-only">T</span>
              {{ hours }}
            </div>
            <div title="Minutter" class="minutes">
              <p>Minutter</p>
              <span class="mobile-only">Min</span>
              {{ minutes }}
            </div>
            <div title="Sekunder" class="seconds">
              <p>Sekunder</p>
              <span class="mobile-only">Sek</span>
              {{ seconds }}
            </div>
          </div>
        </vue-countdown>
      </div>
    </div>
  </div>
  <!-- <div class="spotify">
    <iframe
      style="border-radius: 12px"
      src="https://open.spotify.com/embed/playlist/2gmiGRcHdP1dnw4x6q5pvE?utm_source=generator"
      width="100%"
      height="152"
      frameBorder="0"
      allowfullscreen=""
      allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      loading="lazy"
    ></iframe>
  </div> -->
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
  methods: {},
};
</script>

<style lang="less" scoped>
@background-color: #ffffff;
@text-box-background-color: #b2ac88;
@text-box-text-color: #000000;
@default-font: "Alexis Marie", sans-serif;
@header-font: "Andasia", sans-serif;

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
  &.dynamic-height {
    height: auto;
  }
}

p {
  font-size: 25px;
  font-family: @default-font;
  font-weight: 100;
  text-align: center;
  overflow: visible;
  height: auto;
  &.big {
    font-size: 50px;
  }
  &.header {
    font-size: 60px;
    font-family: @header-font;
    padding-top: 40px;
  }
}

.image-text {
  position: absolute;
  width: 75vw;
  max-width: 1440px;
  left: 50%;
  transform: translate(-50%, 0);
  color: @text-box-text-color;
  overflow: hidden;
  background-color: @text-box-background-color;

  &.bottom {
    bottom: 0%;
    border-radius: 20px 20px 0 0;
    padding: 40px 80px 20px 80px;
    // p {
    //   font-size: 30px;
    //   &.date {
    //     font-size: 50px;
    //   }
    // }
  }
  &.top {
    top: 0%;
    border-radius: 0 0 20px 20px;
    padding: 20px 80px 40px 80px;
  }
}

@media screen and (max-width: 800px) {
  .image-text {
    width: 100%;
    &.bottom,
    &.top {
      border-radius: 0;
      padding: 20px 10px 20px 10px;
    }
  }
}

.center-text {
  top: 0%;
  bottom: 0%;
  left: 50%;
  color: @text-box-text-color;
  padding: 15px;
  background-color: @text-box-background-color;
}

.top-image {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-006-min.jpg");
}

.image-stare {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-001-bw-min.jpg");
}

.spotify {
  position: fixed;
  bottom: 0;
  right: 0;
  z-index: 100;
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
      font-family: @header-font;
    }
    .mobile-only {
      display: none;
      font-family: @header-font;
    }
  }
}

@media screen and (max-width: 1270px) {
  .timer {
    padding-top: 10px;
    div {
      font-size: 46px;
      padding: 0 20px;
      p {
        font-size: 36px;
      }
    }
  }
}

@media screen and (max-width: 1070px) {
  .timer {
    padding-top: 10px;
    div {
      font-size: 40px;
      padding: 0 20px;
      p {
        font-size: 30px;
      }
    }
  }
}

@media screen and (max-width: 975px) {
  .timer {
    padding-top: 10px;
    div {
      font-size: 36px;
      padding: 0 10px;
      p {
        font-size: 26px;
      }
    }
  }
}

@media screen and (max-width: 530px) {
  .timer {
    padding-top: 10px;
    div {
      font-size: 36px;
      padding: 0 12px;
      p {
        font-size: 26px;
        display: none;
      }
      .mobile-only {
        margin-top: -10px;
        font-size: 26px;
        display: block;
      }
    }
  }
}
@media screen and (max-width: 340px) {
  .timer {
    padding-top: 10px;
    div {
      font-size: 30px;
      padding: 0 5px;
      .mobile-only {
        display: none;
      }
    }
  }
}

.flex {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
</style>
