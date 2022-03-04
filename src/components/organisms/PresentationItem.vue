<template>
  <div class="presentation">
    <SocialNetworks />

    <img
      class="presentation-img"
      src="@/assets/images/presentation.svg"
      alt="presentation"
    />
  </div>
</template>

<style scoped>
.presentation {
  position: relative;
  display: grid;
  justify-content: center;
}
.social-networks {
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
}
.presentation-img {
  width: 80%;
  justify-self: center;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'
import { SocialNetworks } from '@/components/molecules'

export default defineComponent({
  components: { SocialNetworks },
})
</script>
