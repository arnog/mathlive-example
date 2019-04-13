<template>
  <div>
    <h3>Mathlive-Component</h3>
    <h1>Euler's Identity</h1>
    <p>$$e^{i\pi} + 1 = 0$$</p>
  </div>
</template>

<script>
import MathLive from "mathlive";

export default {
  name: "mathlivecomponent",
  components: {}
};
//eslint-disable-next-line
console.log("MathLive-Component script called");
MathLive.renderMathInDocument();
</script>
