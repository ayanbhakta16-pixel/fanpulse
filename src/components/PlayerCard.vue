<template>
  <div class="card">
    <h3>{{ player.name }}</h3>

    <p>{{ player.club }}</p>

    <div class="approval">
      Approval: {{ player.approval }}%
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  player: {
    id: number
    name: string
    club: string
    approval: number
    trend: string
  }
}>()
</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 16px;
  margin-bottom: 12px;
}

.approval {
  font-weight: bold;
}
</style>