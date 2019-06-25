<template>
  <div class="layout layout--a">
    <Logo />
    <About />
  </div>
</template>

<script>
// @ is an alias to /src
import Logo from "@/components/logo/Logo.vue";
import About from "@/components/about/About.vue";

export default {
  name: "home",
  components: {
    Logo,
    About
  }
};
</script>
