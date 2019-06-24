<template>
  <div class="app" id="app">
    <Nav />
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
import Nav from "@/components/nav/Nav.vue";
import Footer from "@/components/footer/Footer.vue";

export default {
  name: "App",
  components: {
    Nav,
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
