<template>
  <div class="relative h-full min-h-screen bg-rb-mickeypink">
    <TheNavBar />

    <div class="p-10">
      <router-view />
    </div>
    <div className="relative hidden sm:block z-0">
      <img
        src="/JB.png"
        alt="JB degods"
        className="w-64 fixed -bottom-1 right-10"
      />
    </div>
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar';
import TheFooter from '@/components/gem-farm/TheFooter';
export default {
  components: { TheFooter, TheNavBar },
};
</script>

<style>
input[type='radio']:checked + span {
  @apply text-black;
}
</style>
