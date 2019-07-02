<template>
  <div class="content content--home">
    <Logo />
    <div class="layout layout--style-a">
      <div class="layout__inner">
        <div class="intro">
          <ul class="list list--style-b">
            <li>Freelance frontend developer</li>
            <li>Frontend consultancy</li>
            <li>Bespoke websites</li>
          </ul>
        </div>
      </div>
    </div>
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
