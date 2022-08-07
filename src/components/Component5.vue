<template>
  <div>
    <p> Component 5</p>
  </div>

  <div>
    <h3>Today price: {{coinPrice}}</h3>
    <input type="text" v-model="coinName">
    <button @click="checkPrice(coinName)">Check</button>
  </div>

</template>

<script>
import axios from 'axios'

export default {
  name: "Component-4",
  data() {
    return {
      coinName: "bitcoin",
      coinPrice: 0
    }
  },
  methods: {
    async checkPrice(coinName) {
      const data = await axios
        .get(`https://api.coingecko.com/api/v3/simple/price?ids=${coinName}&vs_currencies=usd`)
        .then(function (response) {
          return response.data;
        })
        .catch(function (error) {
          console.log(error);
        })
      this.coinPrice = data[this.coinName]?.usd;
    }
  }

};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
