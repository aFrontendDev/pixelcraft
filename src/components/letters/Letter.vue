<template>
  <div :class="className(letter)">
    <div
      v-for="n in 80"
      v-bind:key="makeKey(n)"
      :class="makeKey(n)"
      v-on:mouseover="mouseover"
    >
    </div>
  </div>
</template>

<script>
export default {
  name: "Letter",
  props: ["letter"],
  methods: {
    makeKey: count => {
      const num = count;
      const stringA = `a${Math.ceil(num / 10)}`;
      const aTen = (num / 10) % 1 === 0;
      const dec = ((num / 10) % 1).toFixed(1).split(".")[1];
      const endNum = aTen ? 10 : dec;
      const stringB = `-${endNum}`;
      return `block ${stringA}${stringB}`;
    },
    className: letter => {
      return `letter letter--${letter}`;
    },
    transComplete: () => {
      document.documentElement.classList.add("letters-completed");
    },
    mouseover: e => {
      const el = e.target;
      const randomColor = Math.floor(Math.random() * 16777215).toString(16);
      el.style.backgroundColor = `#${randomColor}`;

      setTimeout(() => {
        el.removeAttribute("style");
      }, 5000);
    }
  },
  mounted() {
    setTimeout(() => this.transComplete(), 2350);
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "./_letter.scss";
</style>
