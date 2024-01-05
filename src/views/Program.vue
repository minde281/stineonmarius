<template>
  <div class="full-width">
    <div class="program-holder">
      <div class="center-text">
        <div class="time-table">
          <h1 class="header">Program</h1>
          <div class="timeline">
            <div class="container left">
              <div class="date">12:30</div>
              <i class="icon fa fa-home"></i>
              <div class="content">
                <h2>Oppmøte på Rotvoll Park</h2>
                <p></p>
              </div>
            </div>
            <div class="container right">
              <div class="date">13:00</div>
              <i class="icon fa fa-gift"></i>
              <div class="content">
                <h2>Sermoni</h2>
                <p></p>
              </div>
            </div>
            <div class="container left">
              <div class="date">14:00</div>
              <i class="icon fa fa-user"></i>
              <div class="content">
                <h2>Bobler og kake</h2>
                <p></p>
              </div>
            </div>
            <div class="container right">
              <div class="date">15:00</div>
              <i class="icon fa fa-running"></i>
              <div class="content">
                <h2>Brudeparet drar på fotografering</h2>
                <p></p>
              </div>
            </div>
            <div class="container left">
              <div class="date">16:00</div>
              <i class="icon fa fa-cog"></i>
              <div class="content">
                <h2>Rotvoll park stenges</h2>
                <p></p>
              </div>
            </div>
            <div class="container right">
              <div class="date">16:30</div>
              <i class="icon fa fa-certificate"></i>
              <div class="content">
                <h2>Scandic Nidelven åpnes</h2>
                <p></p>
              </div>
            </div>
            <div class="container left">
              <div class="date">17:00</div>
              <i class="icon fa fa-cog"></i>
              <div class="content">
                <h2>Middagen serveres</h2>
                <p></p>
              </div>
            </div>
            <div class="container right">
              <div class="date">19:00</div>
              <i class="icon fa fa-certificate"></i>
              <div class="content">
                <h2>Dansegulvet åpnes</h2>
                <p></p>
              </div>
            </div>
            <div class="container left">
              <div class="date">01:00</div>
              <i class="icon fa fa-cog"></i>
              <div class="content">
                <h2>Baren stenges</h2>
                <p></p>
              </div>
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
@text-box-text-color: #000000;
@text-box-text-alt-color: #c9b277;
@default-font: "Alexis Marie", sans-serif;
@header-font: "Forum", sans-serif;

.full-width {
  width: 100vw;
  .time-table {
    font-family: @default-font;
    margin: 0 auto;
    .text-right {
      text-align: right;
    }
    .text-left {
      text-align: left;
    }
    .v-col-sm-6.v-col-6.text-right {
      border-right: 1px solid black;
      .border-bottom {
        width: 5px;
        border-bottom: 1px solid black;
      }
    }
  }
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  background: #ffffff;
}

.timeline {
  position: relative;
  width: 100%;
  max-width: 1140px;
  margin: 0 auto;
  padding: 15px 0;
  p {
    font-size: 20px;
  }
}

.timeline::after {
  content: "";
  position: absolute;
  width: 2px;
  background: #000000;
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -1px;
}

.container {
  padding: 15px 30px;
  position: relative;
  background: inherit;
  width: 50%;
}

.container.left {
  left: 0;
}

.container.right {
  left: 50%;
}

.container::after {
  content: "";
  position: absolute;
  width: 16px;
  height: 16px;
  top: calc(50% - 8px);
  right: -8px;
  background: #ffffff;
  border: 2px solid #000000;
  border-radius: 16px;
  z-index: 1;
}

.container.right::after {
  left: -8px;
}

.container::before {
  content: "";
  position: absolute;
  width: 50px;
  height: 2px;
  top: calc(50% - 1px);
  right: 8px;
  background: #000000;
  z-index: 1;
}

.container.right::before {
  left: 8px;
}

.container .date {
  position: absolute;
  display: inline-block;
  top: calc(50% - 8px);
  text-align: center;
  font-size: 14px;
  font-weight: bold;
  color: #000000;
  text-transform: uppercase;
  letter-spacing: 1px;
  z-index: 1;
}

.container.left .date {
  right: -75px;
}

.container.right .date {
  left: -75px;
}

.container .icon {
  position: absolute;
  display: inline-block;
  width: 20px;
  height: 20px;
  padding: 9px 0;
  top: calc(50% - 10px);
  background: @text-box-text-alt-color;
  border: 2px solid #000000;
  border-radius: 40px;
  text-align: center;
  font-size: 18px;
  color: #000000;
  z-index: 1;
}

.container.left .icon {
  right: 56px;
}

.container.right .icon {
  left: 56px;
}

.program-holder .timeline .container .content {
  padding: 30px 90px 30px 30px;
  background: white;
  position: relative;
  border-radius: 0 500px 500px 0;
  text-align: right;
  p {
    text-align: right;
  }
}

.program-holder .timeline .container.right .content {
  padding: 30px 30px 30px 90px;
  border-radius: 500px 0 0 500px;
  text-align: left;
  p {
    text-align: left;
  }
}

.container .content h2 {
  margin: 0 0 0 0;
  font-weight: normal;
  color: #000000;
  font-size: 24px;
}

.container .content p {
  margin: 0;
  line-height: 22px;
  color: #000000;
}

@media (max-width: 767.98px) {
  .timeline::after {
    left: 90px;
  }

  .container {
    width: 100%;
    padding-left: 120px;
    padding-right: 30px;
  }

  .container.right {
    left: 0%;
  }

  .container.left::after,
  .container.right::after {
    left: 82px;
  }

  .container.left::before,
  .container.right::before {
    left: 90px;
    width: 25px;
    border-color: transparent #000000 transparent transparent;
  }

  .container.left .date,
  .container.right .date {
    right: auto;
    left: 25px;
  }

  .container.left .icon,
  .container.right .icon {
    right: auto;
    left: 115px;
  }

  .program-holder .timeline .container.left .content,
  .program-holder .timeline .container.right .content {
    padding: 30px 30px 30px 50px;
    border-radius: 500px 0 0 500px;
    text-align: left;
    p {
      text-align: left;
      font-size: 14px;
    }
    h2 {
      text-align: left;
      font-size: 20px;
    }
  }
}
</style>
