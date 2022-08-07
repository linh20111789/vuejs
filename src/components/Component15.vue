<template>
  <div>
    <p>Component 15</p>
  </div>
  <div>
    <canvas id="chart"></canvas>
  </div>
</template>

<script>
/* eslint-disable */
// import axios from 'axios'
import Chart from "chart.js";
import Chart15Data from "../chart15-data.js";

export default {
  name: "component15",
  data() {
    return {
      Chart15Data: Chart15Data,
    };
  },
  mounted() {
    const ctx = document.getElementById("chart");
    new Chart(ctx, this.Chart15Data);
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.red {
  color: red;
}
</style>
