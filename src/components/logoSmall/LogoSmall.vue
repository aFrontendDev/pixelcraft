<template>
  <router-link class="logo-small" to="/">
    <span class="visually-hidden">PXL</span>
    <div class="logo-small__icons" role="presentation">
      <P />
      <X />
      <L />
    </div>
  </router-link>
</template>

<style lang="scss">
@import "./logosmall.scss";
</style>

<script>
import P from "./P.vue";
import X from "./X.vue";
import L from "./L.vue";

export default {
  name: "LogoSmall",
  components: {
    P,
    X,
    L
  }
};
</script>
