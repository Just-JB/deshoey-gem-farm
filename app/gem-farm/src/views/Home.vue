<template>
  <div class="mb-10">
    <!-- absolute assets -->
    <!-- <div class="absolute hidden sm:block w-20 top-64 xl:left-64 left-8">
      <img src="/40.png" alt="beer" />
    </div>
    <div class="absolute hidden sm:block w-20 top-64 xl:right-64 right-8">
      <img src="/40.png" alt="beer" />
    </div> -->
    <div class="px-16 mt-8 mx-auto max-w-2xl">
      <img src="/DeShoeysbwDEF.png" alt="deshoey" />
    </div>
    <div class="px-16 mt-2 mx-auto max-w-2xl text-center text-lg md:text-3xl">Presented by:</div>
    <div class="sm:flex sm:flex-row items-center justify-between max-w-4xl mx-auto">
      <div class="px-10 sm:px-0">
        <img src="/barrelDAO_logo_black.png" alt="barrelDAO" />
      </div>
      <div class="px-10 text-center text-lg sm:text-3xl w-fit">X</div>
      <div class="max-w-xs md:max-w-sm mx-auto">
        <img src="/mickey_degod_banner.png" alt="mickey degods" />
      </div>
    </div>
    <p class="text-2xl font-bold pt-10">We're no geniuses either, so we made some instructions:</p>
    <p class="pt-5">
      Staking your Shoes, much like drinking beer from them, is a messy process. Here's a quick overview:
      <ol class="pt-5">
        <li>1. Head to our Staking Area and connect your wallet.</li>
        <li>2. Select your Shoes on the left. You may select multiple and move them all over together.</li>
        <li>3. Click the right arrow to stage the NFTs in your vault.</li>
        <li>4. Click "Move NFTs" and sign the transaction to lock them up in the vault.</li>
        <li>5. When you're ready, click "Begin Staking" and sign the final transaction.</li>
        <li>6. Watch those $DUST gainz roll in bruh. You can collect $DUST at any time by clicking the "Collect X $DUST" button.</li>
      </ol>
    </p>
    <p>
      Unstaking is also a trip (turn up your volume for a surprise):
      <ol class="pt-5">
        <li>1. Click "End Staking" and sign the first txn.</li>
        <li>2. Your staking account is now in a "cooldown" state. There's no cooldown period though, so just click "End Cooldown" and sign txn #2.</li>
        <li>3. You may now move your NFTs back into your wallet by selecting them and clicking the left arrow.</li>
        <li>4. Finally, click the "Move NFTs" button to sign the final txn, putting them back in your wallet.</li>
      </ol>
    </p>
  </div>
  <div class="mx-auto">
    <div>
      <!-- <img src='/drink_puddle.png' alt='drink' width='300' /> -->
      <router-link to="farmer">
        <button class="bg-rb-mickeyred text-white rounded-lg py-2 px-3 mx-2">Get Staking</button>
      </router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { GEM_FARM_PROG_ID } from '@gemworks/gem-farm-ts';
export default defineComponent({
  setup() {
    return {
      GEM_FARM_PROG_ID,
    };
  },
});
</script>
<style scoped></style>
