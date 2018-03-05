<template>
  <div>
    <input type="text" v-model="searchText" />
  </div>
</template>

<script>
export default {
  name: 'SearchBox',
  data () {
    return {
      searchText: 'Hello, World'
    }
  }
}
</script>
