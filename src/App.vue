<template>
  <div class="app" id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
@import "@/styles/_global.scss";

.app {
  display: flex;
  width: 100%;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
</style>
