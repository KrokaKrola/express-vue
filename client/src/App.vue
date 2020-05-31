<template>
  <div id="app">
    <Header></Header>
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  components: {
    Header,
  },
};
</script>

<style lang="scss">
  body {
    background-color: #f1f1f1;
    font-family: Roboto, Avenir, Helvetica, Arial, sans-serif;
  }
  .container {
    max-width: 1200px;
    padding: 0 20px;
    width: 100%;
    margin: auto;
  }
</style>
