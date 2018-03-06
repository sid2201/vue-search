<template>
  <div>
    <input class="main-search-box" type="text" placeholder="type to start searching" v-model="searchText" />
  </div>
</template>

<script>
export default {
  name: 'SearchBox',
  data () {
    return {
      searchText: ''
    }
  }
}
</script>

<style scoped>
  .main-search-box {
    font-weight: 100;
    min-width: 300px;
    padding: 7px 15px;
    border: 1px solid #f2f2f2;
    border-radius: 15px;
  }

  .main-search-box:focus {
    outline: none;
    border-color: #32d432;
  }
</style>
