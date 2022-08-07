<template>
  <div>
    <p>Component 11</p>
    <p>link to</p>
  </div>
  <a href="https://vuejs.org" @click.prevent="notify"> A link with e.preventDefault() </a>
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-11",
  data() {
    return {
      someObject: {},
    };
  },
  methods: {
    notify() {
      alert("navigation was prevented.");
    },
  },
  mounted() {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
