<template>
  <div>
    <p>Component 14</p>
  </div>
  <div>
    <canvas id="planet-chart"></canvas>
  </div>
</template>

<script>
/* eslint-disable */
// import axios from 'axios'
import Chart from "chart.js";
import planetChartData from "../planet-data.js";

export default {
  name: "PlanetChart",
  data() {
    return {
      planetChartData: planetChartData,
    };
  },
  mounted() {
    const ctx = document.getElementById("planet-chart");
    new Chart(ctx, this.planetChartData);
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.red {
  color: red;
}
</style>
