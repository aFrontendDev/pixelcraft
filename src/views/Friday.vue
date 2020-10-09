<template>
  <div class="content">
    <div class="layout layout--style-a andrew">
      <div class="layout__inner">
        <div class="video">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/kfVsfOSbJY0?autoplay=1"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>

        <div class="larry">
          <a href="http://shorturl.at/efotU" target="_blank" class="larry-link"
            >The Adventures of Larry Duarte!!!</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "friday",
  components: {},
  methods: {
    init: () => {
      console.log("loaded");
    },
  },
  mounted() {
    setTimeout(() => {
      this.init();
    }, 2350);
  },
};
</script>
