<template>
  <div class="social-networks">
    <SocialLink
      name="Facebook"
      to="https://github.com/joaovmgs"
      icon="facebook.svg"
    />
    <SocialLink
      name="Github"
      to="https://github.com/joaovmgs"
      icon="github.svg"
    />
    <SocialLink
      name="Twitter"
      to="https://github.com/joaovmgs"
      icon="twitter.svg"
    />
  </div>
</template>

<style scoped>
.social-networks {
  display: grid;
  grid-gap: 1rem;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialLink } from '@/components/atoms'

export default defineComponent({
  components: { SocialLink },
})
</script>
