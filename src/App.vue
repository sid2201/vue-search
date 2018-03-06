<template>
  <div id="app">
    <SearchBox></SearchBox>
    <div class="tile-container">
      <template v-for="tile in tile_data">
        <Tile v-bind:key="tile.id" :title="tile.title" ></Tile>
      </template>
    </div>
  </div>
</template>

<script>
import SearchBox from './components/SearchBox'
import Tile from './components/Tile'

export default {
  name: 'App',
  data () {
    return {
      search_text: '',
      tile_data: [
        {
          id: 1,
          title: 'OnePlus'
        },
        {
          id: 2,
          title: 'LG'
        },
        {
          id: 3,
          title: 'Samsung'
        },
        {
          id: 4,
          title: 'Apple'
        },
        {
          id: 5,
          title: 'Nokia'
        },
        {
          id: 6,
          title: 'Blackberry'
        },
        {
          id: 7,
          title: 'ZTE'
        },
        {
          id: 8,
          title: 'HTC'
        },
        {
          id: 9,
          title: 'Sony'
        },
        {
          id: 10,
          title: 'Lenovo'
        }
      ]
    }
  },
  components: {
    SearchBox,
    Tile
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

.tile-container {
  padding: 30px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 0 auto;
}
</style>
