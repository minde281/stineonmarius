<template>
  <div name="side-menu" class="side-menu">
    <v-list>
      <router-link to="/"><v-list-item link>Home</v-list-item></router-link>
      <v-divider></v-divider>
      <router-link to="/new-home">
        <v-list-item link>New home</v-list-item>
      </router-link>
      <router-link to="/program">
        <v-list-item link>Program</v-list-item>
      </router-link>
      <router-link to="/new-home">
        <v-list-item link>New home</v-list-item>
      </router-link>
    </v-list>
  </div>
</template>

<script>
export default {
  name: "side-menu",
  components: {},
  computed: {},
  methods: {},
};
</script>

<style lang="less" scoped>
.side-menu {
  a {
    text-decoration: none;
  }
}
</style>
