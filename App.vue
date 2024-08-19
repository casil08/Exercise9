<template>
  <div id="app">
    <h1>Hello, Vue!</h1>
    <DataComponent />
  </div>
</template>

<script>
import DataComponent from './DataComponent.vue';

export default {
  name: 'App',
  components: {
    DataComponent
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>