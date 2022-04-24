<template>
  <div id="app">
    Hello {{ name }}
    <div v-text="age"></div>
    <div v-html="showAlert"></div>
    <div v-bind:id="bindHeading">Heading</div>

    <div v-bind:class="isRed && 'red'">Binding Classes</div>
    <div v-bind:style="{
      color: color
    }">Binding Styles</div>
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
      bindHeading: "heading",

      isRed: true,
      color: "red"
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

.red {
  color: red;
}
</style>