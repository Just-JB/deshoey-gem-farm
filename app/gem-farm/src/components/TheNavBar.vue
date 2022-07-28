<template>
  <nav class="bg-black flex flex-row justify-center align-middle">
    <NavButton
      v-for="i in menu"
      :key="i.name"
      :title="i.name"
      :url="i.url"
      :class="{ active: path === i.url }"
    />
    <div class="website-button">
      <a href="https://www.deshoeys.xyz/" target="_blank" ref="noreferrer">DeShoeys.xyz</a>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent, computed } from 'vue';
import { useRoute } from 'vue-router';
import NavButton from '@/components/NavButton.vue';

export default defineComponent({
  components: { NavButton },
  setup() {
    const route = useRoute();
    const path = computed(() => route.path);

    const menu = [
      { name: 'Home', url: '/' },
      { name: 'Staking', url: '/farmer' },
      // { name: 'Website', url: 'https://www.deshoeys.xyz/' }
    ];

    return {
      menu,
      path,
    };
  },
});
</script>

<style scoped>
.active {
  @apply bg-white text-black;
}

.more {
  @apply px-10 py-3 text-white
  hover:bg-white hover:text-black;
  outline: none;
}

.website-button {
  @apply px-10 py-3 text-white
  hover:bg-white hover:text-black;
  outline: none;
}
</style>
