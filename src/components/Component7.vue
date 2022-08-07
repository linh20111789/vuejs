<template>
  <div>
    <p> Component 7</p>
  </div>
  <li v-for="item in items" :key="item">
    {{ item.message }}
  </li>
  <li v-for="(item, index) in items" :key="item">
    {{ parentMessage }} - {{ index }} - {{ item.message }}
  </li>
  
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-7",
  data() {
    return {
      parentMessage: 'Parent',
      items: [{ message: 'Foo' }, { message: 'Bar' }]
    }
  },


};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
