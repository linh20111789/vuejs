<template>
  <h3>{{ message }}</h3>
  <Component1 msg="Component 1" />
  <p>-------------------------------------------------------------</p>
  <Component2 />
  <p>-------------------------------------------------------------</p>
  <Component3 @inputData="updateMessage" />
  <p>-------------------------------------------------------------</p>
  <Component4 />
  <p>-------------------------------------------------------------</p>
  <Component5 />
  <p>-------------------------------------------------------------</p>
  <Component6 />
  <p>-------------------------------------------------------------</p>
  <Component7 />
  <p>-------------------------------------------------------------</p>
  <Component8 />
  <p>-------------------------------------------------------------</p>
  <Component9 />
  <p>-------------------------------------------------------------</p>
  <Component10 />
  <p>-------------------------------------------------------------</p>
  <Component11 />
  <p>-------------------------------------------------------------</p>
  <Component12 />
  <p>-------------------------------------------------------------</p>
  <Component13 />
  <p>-------------------------------------------------------------</p>
  <Component14 />
  <p>-------------------------------------------------------------</p>
</template>

<script>
import Component1 from "./components/Component1.vue";
import Component2 from "@/components/Component2.vue";
import Component3 from "./components/Component3.vue";
import Component4 from "./components/Component4.vue";
import Component5 from "./components/Component5.vue";
import Component6 from "./components/Component6.vue";
import Component7 from "./components/Component7.vue";
import Component8 from "./components/Component8.vue";
import Component9 from "./components/Component9.vue";
import Component10 from "./components/Component10.vue";
import Component11 from "./components/Component11.vue";
import Component12 from "./components/Component12.vue";
import Component13 from "./components/Component13.vue";
import Component14 from "./components/Component14.vue";

export default {
  name: "App",
  components: {
    Component1,
    Component2,
    Component3,
    Component4,
    Component5,
    Component6,
    Component7,
    Component8,
    Component9,
    Component10,
    Component11,
    Component12,
    Component13,
    Component14,
  },
  data() {
    return {
      message: "Message default from parent component.",
    };
  },
  methods: {
    updateMessage(mes) {
      this.message = mes;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
