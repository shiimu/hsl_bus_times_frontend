<template>
  <img alt="Hsl logo" src="./assets/logo.png" width="400" height="250" />
  <time-component />
</template>

<script>
import TimeComponent from "./components/TimeComponent.vue";

export default {
  name: "App",
  components: {
    TimeComponent,
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
