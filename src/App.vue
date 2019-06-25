<template>
  <div class="app" id="app">
    <main>
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<style lang="scss">
@import "@/styles/styles.scss";
</style>

<script>
import Footer from "@/components/footer/Footer.vue";

export default {
  name: "App",
  components: {
    Footer
  },
  mounted() {
    this.methodReady();
  },
  methods: {
    methodReady: () => {
      setTimeout(
        () => document.documentElement.classList.add("page-ready"),
        500
      );
    }
  }
};
</script>
