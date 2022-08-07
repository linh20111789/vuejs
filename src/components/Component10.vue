<template>
  <div>
    <p> Component 10</p>
  </div>
  <div v-bind="objectOfAttrs"></div>
  <p> {{count}}</p>
  <button @click="increment">{{ count }}</button>  
</template>

<script>
// import axios from 'axios'

export default {
  name: "Component-10",
  data() {
    return {
      objectOfAttrs: {
        id: 'container',
        class: 'wrapper'
      },
      count: 1,
      someObject: {}
    }
  },
  methods: {
    increment() {
      this.count++
    }
  },
  mounted() {
    const newObject = {}
    this.someObject = newObject

    console.log(newObject === this.someObject) // false
    this.increment()
  
  }
};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
