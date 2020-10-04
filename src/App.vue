<template>
  <div id="app">
    <my-baner />
    <hr />
    <weather />
    <hr />
    <table-al />
  </div>
</template>

<script>
import MyBaner from "./components/MyBaner";
import Weather from "./components/Weather";
import TableAl from "./components/TableAl";

export default {
  name: "App",
  components: {
    MyBaner,
    Weather,
    TableAl,
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
