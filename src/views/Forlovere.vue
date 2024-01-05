<template>
  <div class="full-width">
    <div class="forlovere-holder">
      <div class="center-text">
        <div class="forlovere">
          <h1 class="header">Forlovere</h1>
          <div class="section forlovere">
            <div class="forlover">
              <h2>Stines forlover - Sandra Gundersen</h2>
              <img
                src="https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Sandra+forlover.jpg"
                alt="Sandra, Stines forlover"
              />
              <h5>Dette sier Stine om Sandra:</h5>
              <p>
                Sandra og jeg ble kjent i 8. klasse da vi startet på samme
                ungdomsskole og havnet i samme vennegjeng, med blant annet Lise,
                Ina og Tonje (si hei til dem i bryllupet og jeg lover dere god
                stemning og dynamitedans). <br /><br />
                Vi rakk ikke å bli veldig godt kjent før Sandra flyttet til
                England samme jul, men vi holdt kontakten over MSN. Da hun
                flyttet tilbake var vi sammen hver eneste dag og siden har vi
                opplevd veldig mye sammen. Vi var gjester i hverandres
                konfirmasjoner og sommeren etter reiste vi på vår første tur
                sammen, til Hellas. Senere samme sommer var vi også på en
                bondegård på Leka. Vi skulle passe på kalvene, men de klarte å
                rømme. Noen år senere, på en tur til Russland, våknet vi av
                skudd utenfor vinduet, men begge var for trøtte til å stå opp,
                forstå det den som kan. <br /><br />
                Vi fikk begge barn i samme tid, så nå går det mer i playdates
                enn kalvejakt, og selv om MSN er nedlagt sender vi daglig flere
                meldinger. Da Sandra giftet seg i 2021 fikk jeg æren av å være
                forlover. <br /><br />
                Si gjerne hei til Sandra på bryllupet. Du kan mest sannsynlig
                finne henne på dansegulvet.
              </p>
            </div>
            <div class="forlover">
              <h2>Marius' forlover - Tom Erik Berger</h2>
              <img
                src="https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tom+Erik+Forlover.jpg"
                alt="Tom Erik, Marius's forlover"
              />
              <h5>Dette sier Marius om Tom Erik:</h5>
              <p>
                Tom Erik og jeg møttes på barneskolen gjennom et par felles
                bekjente. Vi ble fort en gjeng som holdt sammen gjennom hele
                ungdomsskolen. Da vi var ferdig på ungdomsskolen ble vi splittet
                opp til hver vår videregående skole. <br /><br />
                Selv om gjengen ikke møttes så ofte da vi gikk på videregående,
                møttes Tom Erik og jeg god en del. Vi hadde en stor felles
                interesse for spillet Tibia og har sannsynligvis noen tusen
                timer i dette spillet begge to. <br /><br />
                Den senere tiden har vi møttes en del mindre enn vi gjorde før
                særlig da vi fikk barn, men hver gang vi møtes er det som om
                ingen tid har gått og vi kan sitte i timesvis og snakke om alt
                og ingenting.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({}),
  computed: {},
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

.forlovere {
  max-width: 1152px;
  width: 90vw;
  text-align: center;
  h5 {
    font-family: @header-font;
    color: @text-box-text-alt-color;
    font-weight: 200;
    font-size: 24px;
    margin-bottom: 0;
  }
}

img {
  width: 100%;
  margin-bottom: 20px;
}

.forlover {
  margin-bottom: 40px;
}

@media screen and (max-width: 480px) {
  .forlovere {
    h5 {
      font-size: 18px;
    }
  }
}
</style>
