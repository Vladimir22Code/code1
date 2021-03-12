<template>
  <div class="board">
    <field></field>
  </div>
</template>

<script>
import Field from './Field.vue'

export default {
  components: {
    Field
    }, 
}
</script>

<style scoped>
.board {
  margin: 50px auto;
  width: 480px;
  height: 480px;
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-template-rows: repeat(8, 1fr);
}
</style>