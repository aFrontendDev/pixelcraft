<template>
  <div class="content">
    <div class="layout layout--style-a">
      <div class="layout__inner">
        <Title main="About" />
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
import Title from "@/components/title/Title.vue";

export default {
  name: "about",
  components: {
    About,
    Experience,
    Availability,
    Title
  }
};
</script>
