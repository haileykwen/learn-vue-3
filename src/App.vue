<template>
  <div id="app">
    Hello {{ name }}
    <div v-text="age"></div>
    <div v-html="showAlert"></div>
    <div v-bind:id="bindHeading">Heading</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: "harleykwen",
      age: 22,
      showAlert: `<a href="#" onclick="alert('this is html binding')">Click here to show html binding</a>`,
      bindHeading: "heading"
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

#heading {
  background-color: blue;
}
</style>