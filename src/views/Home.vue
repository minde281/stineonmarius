<template>
  <div class="full-width background-image top-image">
    <div class="image-text bottom">
      <h1>Vi gifter oss 22. juni 2024</h1>
      <h2>Bli med å feire dagen med oss</h2>
    </div>
  </div>
  <div class="full-width the-day">
    <div class="center-text">
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
      <h1>Lorem, ipsum dolor sit amet</h1>
      <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit.</h2>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #b2ac88;
}

.background-image {
  background-color: #b2ac88;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.full-width {
  height: calc(~"100vh - 150px");
  width: 100vw;
  max-width: 1920px;
  position: relative;
  background-color: #b2ac88;
}

.image-text {
  position: absolute;
  width: 75vh;
  left: 50%;
  transform: translate(-50%, 0);
  color: #000000;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 100;
  text-align: center;
  overflow: visible;
  height: auto;
  background-color: #969696;

  &.bottom {
    bottom: 0%;
    border-radius: 20px 20px 0 0;
    padding: 40px 80px 20px 80px;
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
  color: #000000;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 100;
  text-align: center;
  overflow: visible;
  height: auto;
  background-color: #969696;
}

.top-image {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-006.jpg");
}

.image-stare {
  background-image: url("https://s3.eu-west-1.amazonaws.com/mariusminde.no/stineogmarius/Tyrkia2013-001-bw.jpg");
}
</style>
