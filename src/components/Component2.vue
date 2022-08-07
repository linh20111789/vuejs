<template>
  <div class="hello">
    <p>
      Component 2
    </p>
  <div>
  </div>
    <h1>{{ reversedMessage }}</h1>
  </div>
</template>

<script>
export default {
  name: 'component-2',
  data(){
    return {
      message: "hững hờ mai thoảng gió đưa hương"
    }
  },
  computed: {
    reversedMessage() {
      return this.message.split(' ').reverse().join(' ')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
