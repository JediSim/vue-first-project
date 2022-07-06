<template lang="">
  <div>
    <ul v-for="(row, index) in grid" :key="index">
      <ul v-for="(cell, i) in row" :key="i">
        <li>{{ cell }}</li>
      </ul>
    </ul>
  </div>
</template>
<script>
export default {
  name: "TicTacToeGrid",
  data() {
    return {
      grid: [
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
      ],
      player: 1,
      winner: 0,
    };
  },
};
</script>
<style lang="" scoped></style>
