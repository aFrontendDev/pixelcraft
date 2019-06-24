<template>
  <nav class="nav">
    <router-link class="nav__link" to="/">Home</router-link>
    <router-link class="nav__link" to="/about">About</router-link>
  </nav>
</template>

<style lang="scss">
@import "./nav.scss";
</style>

<script>
export default {
  name: "Nav"
};
</script>
