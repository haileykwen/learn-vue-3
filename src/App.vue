<template>
  <div id="app">
    Hello {{ name }}
    <div v-text="age"></div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: "harleykwen",
      age: 22
    };
  }
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