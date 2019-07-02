<template>
  <nav class="nav">
    <LogoSmall />
    <router-link class="nav__link" to="/">Home</router-link>
    <router-link class="nav__link" to="/about">About</router-link>
  </nav>
</template>

<style lang="scss">
@import "./nav.scss";
</style>

<script>
import LogoSmall from "@/components/logoSmall/LogoSmall.vue";

export default {
  name: "Nav",
  components: {
    LogoSmall
  }
};
</script>
