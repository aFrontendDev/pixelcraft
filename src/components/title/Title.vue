<template>
  <div class="page-title">
    <h1 class="page-title__main">{{main}}</h1>
  </div>
</template>

<style lang="scss">
@import "./title.scss";
</style>

<script>

export default {
  name: "Title",
  props: ["main"]
};
</script>
