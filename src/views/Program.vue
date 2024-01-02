<template>
  <div class="full-width">
    <div class="program-holder">
      <div class="center-text">
        <div class="time-table">
          <h1 class="header">Program</h1>
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

.full-width {
  width: 100vw;
  .time-table {
    font-family: @default-font;
    width: 80vw;
    margin: 0 auto;
    .header {
      font-family: @header-font;
      color: @text-box-text-alt-color;
      font-size: 3rem;
      font-weight: 200;
      margin-bottom: 2rem;
      text-align: center;
    }
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
</style>
