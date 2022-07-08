<template>
  <div class="relative h-full min-h-screen bg-rb-mickeypink">
    <TheNavBar />
    <div class="absolute w-20 top-20 left-64">
      <img src="/40.png" alt="beer" />
    </div>
    <div class="absolute w-20 top-20 right-64">
      <img src="/40.png" alt="beer" />
    </div>
    <div class="px-16 mt-2 mx-auto max-w-2xl">
      <img src="/barrelDAO_logo_black.png" alt="barrelDAO" />
    </div>
    <div class="px-16 mt-2 mx-auto max-w-2xl text-center text-3xl">
      X
    </div>
    <div class="px-16 mt-2 mx-auto max-w-2xl">
      <img src="/DeShoeysbwDEF.png" alt="deshoey" />
    </div>

    <div class="p-10">
      <router-view />
    </div>
    <div className="relative hidden sm:block z-0">
      <!-- <img
        src="/drink_puddle.png"
        alt="Drink Puddle"
        className=" w-52 fixed bottom-0 left-10"
      /> -->
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
