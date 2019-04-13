<template>
  <div id="app">
    <MathLiveComponent></MathLiveComponent>
  </div>
</template>

<script>
import MathLiveComponent from "./components/MathLiveComponent.vue";

export default {
  name: "app",
  components: {
    MathLiveComponent
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
