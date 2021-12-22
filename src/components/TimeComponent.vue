<template>
  <div>
    <ul class="list-group">
      <li class="list-group-item" v-show="isDate">
        <strong></strong> {{ date }}
      </li>
      <li class="list-group-item" v-show="isTime">
        <strong></strong> {{ time }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "TimeComponent",
  data: () => ({
    date: "",
    time: "",
    isDate: true,
    isTime: true,
  }),
  methods: {
    printDate: function () {
      return new Date().toLocaleDateString();
    },
    printTime: function () {
      return new Date().toLocaleTimeString();
    },
  },
  mounted: function () {
    this.date = this.printDate();
    this.time = this.printTime();
  },
};
</script>
