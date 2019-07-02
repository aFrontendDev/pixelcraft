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
import Footer from "@/components/footer/Footer.vue";
import Nav from "@/components/nav/Nav.vue";

export default {
  name: "App",
  components: {
    Footer,
    Nav
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
