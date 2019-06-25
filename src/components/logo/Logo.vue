<template>
  <div class="logo">
    <h1 class="visually-hidden">Pixel Craft</h1>
    <div class="word-container" role="presentation">
      <div class="para">
        <Letter letter="p" />
        <Letter letter="i" />
        <Letter letter="x" />
        <Letter letter="e" />
        <Letter letter="l" />
      </div>
      <div class="para">
        <Letter letter="c" />
        <Letter letter="r" />
        <Letter letter="a" />
        <Letter letter="f" />
        <Letter letter="t" />
      </div>
    </div>
  </div>
</template>

<script>
import Letter from "../letters/Letter.vue";

export default {
  name: "Logo",
  props: {
    msg: String
  },
  components: {
    Letter
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "./_logo.scss";
</style>
