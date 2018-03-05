<template>
  <div id="app">
    <SearchBox></SearchBox>
  </div>
</template>

<script>
import SearchBox from './components/SearchBox'

export default {
  name: 'App',
  components: {
    SearchBox
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
