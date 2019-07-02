<template>
  <div class="content">
    <div class="layout layout--style-a">
      <div class="layout__inner">
        <About />
        <Experience />
        <Availability />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import About from "@/components/about/About.vue";
import Experience from "@/components/experience/Experience.vue";
import Availability from "@/components/availability/Availability.vue";

export default {
  name: "about",
  components: {
    About,
    Experience,
    Availability
  }
};
</script>
