<template>
  <div>
    <p> Component 3</p>
    <input
      placeholder="Enter Text Here"
      v-model="tempMessage"
    />
    <div>
      <button @click="sendMessage">@Emit event</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ComponentFirst",
  data() {
    return {
      tempMessage: ''
    }
  },
  methods: {
    sendMessage() {
      this.$emit('inputData', this.tempMessage);
      this.tempMessage = '';
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
