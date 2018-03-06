<template>
    <div class="tile">
        <div>{{ this.title }}</div>
    </div>
</template>

<script>
export default {
  name: 'Tile',
  props: ['title']
}
</script>

<style scoped>
    .tile {
        width: 200px;
        height: 200px;
        border: 1px solid #f2f2f2;
        border-radius: 5px;
        margin-bottom: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: lightgrey;
    }
</style>
