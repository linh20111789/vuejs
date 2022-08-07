<template>
  <div>
    <p> Component 9</p>
  </div>
  <li v-for="n in evenNumbers" :key="n">
    {{ n }}
  </li>
  <ul v-for="numbers in sets" :key="numbers">
    <li v-for="n in even(numbers)" :key="n">
      {{ n }}
    </li>
</ul>  
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-8",
  data() {
    return {
      numbers: [1, 2, 3, 4, 5],
      sets: [[ 1, 2, 3, 4, 5 ], [6, 7, 8, 9, 10]]
    }
  },
  computed: {
    evenNumbers() {
      return this.numbers.filter(n => n % 2 === 0)
    }
  },
  methods: {
    even(numbers) {
      return numbers.filter(number => number % 2 === 0)
    }
  }

};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
