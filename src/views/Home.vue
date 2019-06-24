<template>
  <div class="layout layout--a">
    <Logo />
  </div>
</template>

<script>
// @ is an alias to /src
import Logo from "@/components/logo/Logo.vue";

export default {
  name: "home",
  components: {
    Logo
  }
};
</script>
