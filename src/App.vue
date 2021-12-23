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
