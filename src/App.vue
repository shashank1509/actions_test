<template>  
  <RandomNumber msg="Welcome to Unit Testing with Vue" />
  <h2>This change is auto deployed on a push</h2>
</template>

<script>
import RandomNumber from './components/RandomNumber.vue'

export default {
  name: 'App',
  components: {
    RandomNumber
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
