<template>
  <div v-for="field in $store.state.fields" 
  :key="field.id" 
  :class="field.color">
  <piece v-if="field.display">
    <img class="piece" :src="field.display">
  </piece>
  </div>
</template>

<script>
import Piece from './Piece.vue'

export default {
  components: {
    Piece
    }
}
</script>

<style scoped>
  .light {
  display: grid;
  background-color: var(--light);
  width: 60px;
  height: 60px;
  place-items: center;
  }
  
  .dark {
  display: grid;
  background-color: var(--dark);
  width: 60px;
  height: 60px;
  place-items: center;
  }

  .piece {
  width: 42px;
  height: 42px;
  }
</style>