<template>
  <div>
    <p> Component 6</p>
  </div>
  <div>
    <h3 v-if="status">You can see this message.</h3>
  </div>
  <div>
    <h3 v-if="grade >= 3.2">You are excellent!</h3>
    <h3 v-else-if="2.5 <= grade && grade < 3.2">You are quite good!</h3>
    <h3 v-else>it's only just begun!</h3>
  </div>
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-6",
  data() {
    return {
      status: true,
      grade: 4
    }
  },


};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
