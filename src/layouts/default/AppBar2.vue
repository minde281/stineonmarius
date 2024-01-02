<template>
  <v-btn @click="sideMenuOpen = !sideMenuOpen" class="float-right on-top">
    <v-icon icon="mdi-menu"></v-icon>
  </v-btn>
  <v-navigation-drawer
    location="right"
    color="header"
    app
    temporary
    v-model="sideMenuOpen"
  >
    <div class="side-menu">
      <div class="close-menu-holder">
        <v-btn @click="sideMenuOpen = !sideMenuOpen">
          <v-icon icon="mdi-close"></v-icon>
        </v-btn>
      </div>
      <v-list>
        <router-link to="/"><v-list-item link>Home</v-list-item></router-link>
        <v-divider></v-divider>
        <router-link to="/new-home">
          <v-list-item link>New home</v-list-item>
        </router-link>
        <router-link to="/program">
          <v-list-item link>Program</v-list-item>
        </router-link>
        <router-link to="/faq">
          <v-list-item link>FAQ</v-list-item>
        </router-link>
      </v-list>
    </div>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "AppBar",
  data() {
    return {
      sideMenuOpen: false,
    };
  },
  created() {},
  methods: {},
};
</script>

<style scoped>
.float-right {
  position: fixed;
  right: 15px;
  top: 1px;
  margin: 1rem;
  font-size: 20px;
}

.on-top {
  z-index: 1000;
}

.close-menu-holder {
  display: flex;
  justify-content: flex-end;
  margin: 1rem;
}
nav {
  font-family: "Alexis Marie";
}
a {
  text-decoration: none;
  color: #000000;
}
.router-link-exact-active > div {
  background-color: #c9b277;
}
</style>

<style lang="less"></style>
