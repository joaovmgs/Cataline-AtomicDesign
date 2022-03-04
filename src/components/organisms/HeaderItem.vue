<template>
  <header class="header">
    <Logo />
    <NavBar />
    <SearchBar />
  </header>
</template>

<style scoped>
.header {
  width: 100%;
  display: grid;
  grid-template-columns: 200px repeat(2, auto);
  align-items: center;
  justify-content: space-between;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'
import { NavBar, SearchBar } from '@/components/molecules'
import { Logo } from '@/components/atoms'

export default defineComponent({
  components: { NavBar, SearchBar, Logo },
})
</script>
