<template>
  <div>
    <p>Component 12</p>
  </div>
  <p :class="{ red: isRed }" @click="toggleRed">
    This should be red... but click me to toggle it.
  </p>

  <!-- style bindings also support object and arrays -->
  <p :style="{ color }" @click="toggleColor">
    This should be green, and should toggle between green and blue on click.
  </p>
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-12",
  data() {
    return {
      message: "Hello World!",
      isRed: true,
      color: "green",
    };
  },
  methods: {
    toggleRed() {
      this.isRed = !this.isRed;
    },
    toggleColor() {
      this.color = this.color === "green" ? "blue" : "green";
    },
  },
  mounted() {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.red {
  color: red;
}
</style>
