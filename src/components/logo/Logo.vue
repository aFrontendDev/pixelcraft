<template>
  <div class="logo">
    <Letter letter="p" />
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
