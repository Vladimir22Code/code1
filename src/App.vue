<template>
  <board></board>
</template>

<script>
import Board from './components/Board.vue'

export default {
  components: {
    Board
  },
}
</script>

<style>
  :root {
    --light: #e3d18a;
    --dark: #9e7540;
  }

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
