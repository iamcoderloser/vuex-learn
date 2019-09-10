<template>
  <div id="app">
    <h1>{{count}}</h1>
    <HelloWorld></HelloWorld>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import { mapState } from "vuex";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data() {
    return {};
  },
  computed: {
    ...mapState(["count"])
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
