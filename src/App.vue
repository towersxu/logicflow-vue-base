<template>
  <div id="app">
    <Lf />
  </div>
</template>

<script>
import Lf from "./components/Lf";

export default {
  name: "App",
  components: {
    Lf,
  },
};
</script>

<style>
html,
body {
  width: 100%;
  height: 100%;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  width: 100%;
  height: 100%;
}
</style>
