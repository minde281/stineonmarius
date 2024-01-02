<template>
  <div class="the-day">
    <div class="content">
      <div class="center-text">
        <div class="section sermoni">
          <h1 class="header">Sermoni</h1>
          <p>Rotvoll Park</p>
          <p>Arkitekt Ebbells veg 22</p>
          <p>7053 Ranheim</p>
          <p>Bygg D, kl 14.00</p>
          <p></p>
          <br />
          <p>
            Etter&nbsp;sermonien&nbsp;blir&nbsp;det
            servert&nbsp;bobler&nbsp;og&nbsp;kake.
          </p>
          <p>
            De&nbsp;som&nbsp;ønsker&nbsp;kan&nbsp;være&nbsp;på
            Rotvoll&nbsp;Park&nbsp;frem&nbsp;til&nbsp;kl&nbsp;16.00
          </p>
        </div>
        <div class="section">
          <h1 class="header">Selskap</h1>
          <p>Scandic Nidelven</p>
          <p>Havnegata 1-3</p>
          <p>7010 Trondheim</p>
          <p>Kl 17.00</p>
          <p></p>
          <br />
          <p>Det serveres aperitiff,</p>
          <p>3-retters middag med drikke og kaffe.</p>
          <p>Ønskes noe utover dette kan det kjøpes i baren.</p>
        </div>
      </div>
    </div>
  </div>
  <div class="img-holder">
    <img
      src="https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/ring11-min.png"
      alt="Ring"
    />
  </div>
  <div class="practical-info">
    <div class="content">
      <div class="center-text">
        <div class="section overnatting">
          <p class="header">Overnatting TODO</p>
          <p>
            Ønsker dere å overnatte på hotellet kan dere bruke rabattkode
            "RABATTKODE" ved bestilling.
          </p>
          <p>Da er Norges beste hotellfrokost inkludert.</p>
        </div>
        <div class="section toastmaster">
          <p class="header">Toastmaster TODO</p>
          <p>Vi har gleden av å presentere vår toastmaster</p>
          <p>{{ toastmaster.name }}</p>
          <br />
          <p>
            Dersom&nbsp;du&nbsp;har&nbsp;noe&nbsp;du&nbsp;ønsker&nbsp;å fortelle
            felleskapet&nbsp;kan&nbsp;du&nbsp;kontakte
            {{ toastmaster.name }}&nbsp;på tlf:&nbsp;{{ toastmaster.phone }}.
          </p>
          <p>Vi vil likevel be dere holde taler korte og underholdende</p>
        </div>
        <div class="section rsvp">
          <p class="header">RSVP</p>
          <p>
            Gi&nbsp;gjerne&nbsp;beskjed&nbsp;om&nbsp;dere&nbsp;kommer
            eller&nbsp;ikke&nbsp;innen&nbsp;15.&nbsp;april.
          </p>
          <p>Tlf&nbsp;Stine: 47898727</p>
          <p>Tlf&nbsp;Marius: 98401479</p>
        </div>
      </div>
    </div>
  </div>
  <div class="img-holder">
    <img
      src="https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/wedding bouquet7-min.png"
      alt="Brudebukett"
    />
  </div>
  <div class="photo-and-music">
    <div class="content">
      <div class="center-text">
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
</template>

<script>
export default {
  data: () => ({
    toastmaster: {
      name: "Stine Minde",
      phone: "81549300",
    },
  }),
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
@text-box-text-alt-color: #c9b277;
@default-font: "Alexis Marie", sans-serif;
@header-font: "Forum", sans-serif;

.img-holder {
  max-width: 80vw;
  margin: 0 auto;
  overflow: hidden;
  position: relative;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}

.content {
  .center-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    .section {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      margin: 1rem;
      padding: 1rem;
      width: 100%;
      max-width: 600px;
      p {
        font-family: @default-font;
        font-size: 24px;
        font-weight: 200;
        margin: 0;
        text-align: center;
      }
      a {
        color: @text-box-text-alt-color;
      }
    }
  }
}
</style>
