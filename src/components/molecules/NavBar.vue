<template>
  <nav class="nav-bar">
    <NavItem text="Home" to="https://google.com" />
    <NavItem text="Sobre" to="https://google.com" />
    <NavItem text="Contato" to="https://google.com" />
    <NavItem text="Serviços" to="https://google.com" />
  </nav>
</template>

<style scoped>
.nav-bar {
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'
import { NavItem } from '@/components/atoms'

export default defineComponent({
  components: { NavItem },
})
</script>
