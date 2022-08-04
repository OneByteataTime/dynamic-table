<template>
  <div id="app">
    <h2>Dynamic Table Example</h2>
    <Coverages />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Coverages from './components/Coverages.vue';

export default Vue.extend({
  name: 'App',
  components: {
    Coverages
  }
});
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
