<template>
  <div class="homepage">
    <h1>FanPulse</h1>

    <p>The public approval tracker for sports.</p>

    <h2>Most Loved ❤️</h2>

    <PlayerCard
      v-for="player in players"
      :key="player.id"
      :player="player"
    />
  </div>
</template>

<script setup lang="ts">
import PlayerCard from '../components/PlayerCard.vue'
import { players } from '../mock/players'
</script>

<style scoped>
.homepage {
  max-width: 900px;
  margin: 0 auto;
  padding: 24px;
}
</style>