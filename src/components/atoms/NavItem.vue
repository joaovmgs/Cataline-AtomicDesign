<template>
  <a :href="to" class="nav-item"> {{ text }}</a>
</template>

<style scoped>
.nav-item {
  color: #293947;
  text-decoration: none;
  font-size: 1.3rem;
}
</style>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    text: {
      type: String,
      require: true,
    },
    to: {
      type: String,
      require: true,
    },
  },
})
</script>
