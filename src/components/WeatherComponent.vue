<template>
  <weather></weather>
</template>

<script>
export default {
  name: "TimeComponent",
  data: () => ({
    time: "",
    isTime: true,
  }),
  methods: {
    printTime: function () {
      return new Date().toLocaleTimeString([], {
        hour: "2-digit",
        minute: "2-digit",
      });
    },
  },
  mounted: function () {
    this.time = this.printTime();
  },
};
</script>
