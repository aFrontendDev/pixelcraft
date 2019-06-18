<template>
  <div :class="className(letter)">
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a1')" :class="classCount(n, 'a1')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a2')" :class="classCount(n, 'a2')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a3')" :class="classCount(n, 'a3')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a4')" :class="classCount(n, 'a4')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a5')" :class="classCount(n, 'a5')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a6')" :class="classCount(n, 'a6')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a7')" :class="classCount(n, 'a7')"></div>
    <div v-for="n in 10" v-bind:key="makeKey(n, 'a8')" :class="classCount(n, 'a8')"></div>
  </div>
</template>

<script>
export default {
  name: "Letter",
  props: ["letter"],
  methods: {
    makeKey: (count, string) => {
      return `${string}-${count}`;
    },
    classCount: (count, string) => {
      return `${string}-${count}`;
    },
    className: letter => {
      return `letter letter--${letter}`;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "./_letter.scss";
</style>
