<template>
  <a class="social-link" :href="to">
    <img :src="require(`@/assets/images/icons/${icon}`)" :alt="name" />
  </a>
</template>

<style scoped>
.social-link {
  background-color: #ff895f;
  width: 47px;
  height: 47px;
  border-radius: 5rem;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
}
.social-link img {
  width: 23px;
  height: 23px;
}
.social-link:hover {
  transform: scale(1.1);
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  computed: {
    iconPath(): string {
      return require(`@/assets/images/icons/${this.icon}`)
    },
  },
  props: {
    name: { Type: String, required: true },
    to: { Type: String, required: true },
    icon: { Type: String, required: true },
  },
})
</script>
