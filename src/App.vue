
<template>
  <div id="app">
    <h1>{{ message }}</h1>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
  },
  data() {
    return {
      message: ''
    }
  },
  mounted() {
    const result = window.myLibrary.add(5, 3);
    this.message = `Result of add(5, 3): ${result}`;
  }
}
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
