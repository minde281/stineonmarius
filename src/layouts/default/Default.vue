<template>
  <v-app>
    <div class="container">
      <default-bar />
      <div class="top-img-holder">
        <img
          src="https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-006-min.jpg"
          alt="Bilde av Stine og Marius hvor det ser ut som de er glad i hverandre"
        />
        <div class="img-text">
          <h1 class="main-header">Stine & Marius</h1>
          <h2>22.06.2024</h2>
        </div>
      </div>
      <default-view />
    </div>
  </v-app>
</template>

<script setup>
import DefaultBar from "./AppBar2.vue";
import DefaultView from "./View.vue";
</script>

<style lang="less">
@font-face {
  font-family: "Forum";
  src: url("/fonts/Forum-Regular.ttf") format("truetype");
}

@font-face {
  font-family: "Alexis Marie";
  src: url("/fonts/Alexis Marie.ttf") format("truetype");
}

@background-color: #ffffff;
@text-box-background-color: #b2ac88;
@text-box-text-color: #000000;
@text-box-text-alt-color: #c9b277;
@default-font: "Alexis Marie", sans-serif;
@header-font: "Forum", sans-serif;

.float-right {
  position: fixed;
  right: 30px;
  top: 40px;
  margin: 1rem;
  font-size: 20px;
}

.header {
  font-family: @header-font;
  color: @text-box-text-alt-color;
  font-size: 60px;
  font-weight: 200;
  margin-bottom: 10px;
  text-align: center;
}

p {
  font-family: @default-font;
  font-size: 24px;
  font-weight: 200;
  margin: 0;
  text-align: center;
  strong {
    font-weight: 600;
  }
}

h2 {
  font-family: @header-font;
  color: @text-box-text-alt-color;
  font-size: 36px;
  font-weight: 200;
  text-align: center;
}

a {
  color: @text-box-text-alt-color;
}

@media screen and (max-width: 480px) {
  .header {
    font-size: 2rem;
    margin-bottom: 5px;
  }
  p {
    font-size: 16px;
  }
  h2 {
    font-size: 24px;
  }
}
</style>

<style lang="less" scoped>
@background-color: #ffffff;
@text-box-background-color: #b2ac88;
@text-box-text-color: #000000;
@text-box-text-alt-color: #c9b277;
@default-font: "Alexis Marie", sans-serif;
@header-font: "Forum", sans-serif;
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #ffffff;
}

.top-img-holder {
  width: 100vw;
  min-height: 50vh;
  max-height: 70vh;
  margin: 0 auto;
  overflow: hidden;
  position: relative;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .img-text {
    position: absolute;
    top: 80%;
    left: 50%;
    transform: translate(-50%, -50%);
    h1,
    h2,
    h3,
    h4,
    h5,
    h6 {
      font-family: @header-font;
      font-weight: 200;
      color: @text-box-text-color;
      text-align: center;
      margin: 0;
    }
    .main-header {
      font-size: 72px;
      font-weight: 200;
      margin-bottom: 0.5rem;
    }
    h2 {
      font-size: 48px;
    }
  }
}

@media (max-width: 1200px) {
  .top-img-holder {
    .img-text {
      .main-header {
        font-size: 64px;
      }
      h2 {
        font-size: 40px;
      }
    }
  }
}

@media (max-width: 1000px) {
  .top-img-holder {
    .img-text {
      .main-header {
        font-size: 48px;
      }
      h2 {
        font-size: 32px;
      }
    }
  }
}

@media (max-width: 600px) {
  .top-img-holder {
    .img-text {
      .main-header {
        font-size: 32px;
      }
      h2 {
        font-size: 24px;
      }
    }
  }
}

@media (max-width: 400px) {
  .top-img-holder {
    .img-text {
      .main-header {
        font-size: 24px;
      }
      h2 {
        font-size: 16px;
        margin-bottom: 5px;
      }
    }
  }
}
</style>
