<template>
  <div id="app">
    <h1>Hello</h1>
    $$e^{i\pi} + 1 = 0$$
    <MathLiveComponent v-model="formula" v-on:input="input()"
      >g(x)=</MathLiveComponent
    >
    <div id="output">{{ formula }}</div>
  </div>
</template>

<script>
import { renderMathInDocument } from "mathlive";
import MathLiveComponent from "./components/MathLiveComponent.vue";

export default {
  name: "app",
  components: {
    MathLiveComponent,
  },
  data: function() {
    return { formula: "h(x)" };
  },
  mounted: function() {
    renderMathInDocument();
  },
  methods: {
    input: function() {
      // eslint-disable-next-line
      console.log(this.formula);
    },
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
