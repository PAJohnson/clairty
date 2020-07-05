<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4rem;
}

#app {
  background-image: url("./assets/bg.jpg");
  background-position: center; /* Center the image */
  background-repeat: no-repeat; /* Do not repeat the image */
  background-size: cover; /* Resize the background image to cover the entire container */
  height: 100vh;
}
</style>
