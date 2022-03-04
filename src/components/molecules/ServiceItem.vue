<template>
  <div class="service">
    <h2>{{ title }}</h2>
    <p class="description">{{ description }}</p>
  </div>
</template>

<style scoped>
.service h2 {
  color: #935e92;
  font-weight: bold;
  margin-bottom: 0.8rem;
}
.description {
  color: #293947;
  line-height: 1.5;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    title: { Type: String, required: true },
    description: { Type: String, required: true },
  },
})
</script>
