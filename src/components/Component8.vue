<template>
  <div>
    <p> Component 8</p>
  </div>
  <ul>
    <li v-for="value in myObject" :key="value">
      {{ value }}
    </li>

    <li v-for="(value, key, index) in myObject" :key="key">
      {{ index }}. {{ key }}: {{ value }}
    </li>
  </ul>
  
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-8",
  data() {
    return {
      myObject: {
        title: 'How to do lists in Vue',
        author: 'Jane Doe',
        publishedAt: '2016-04-10'
      }
    }
  },


};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
