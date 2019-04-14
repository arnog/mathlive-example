<template>
  <div id="app">
    $$e^{i\pi} + 1 = 0$$
    <MathLiveComponent></MathLiveComponent>
  </div>
</template>

<script>
import MathLive from "mathlive";
import MathLiveComponent from "./components/MathLiveComponent.vue";

export default {
  name: "app",
  components: {
    MathLiveComponent
  },
  mounted: function() {
    MathLive.renderMathInDocument();
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
