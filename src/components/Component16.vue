<template>
  <div>
    <p>Component 16</p>
  </div>
  <ol>
    <li v-for="todo in todos" :key="todo">
      {{ todo.text }}
    </li>
  </ol>
</template>

<script>
/* eslint-disable */
// import axios from 'axios'
import Chart from "chart.js";
import Chart15Data from "../chart15-data.js";

export default {
  name: "component16",
  data() {
    return {
      Chart15Data: Chart15Data,
      todos: [
        { text: "Học JavaScript" },
        { text: "Học Vue" },
        { text: "Xây dựng cái gì đó hay ho" },
      ],
      showMessage: function () {
        console.log(this.todos);
      },
    };
  },
  created() {
    console.log(this.Chart15Data);
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
