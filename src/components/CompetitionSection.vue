<script setup>
import { ref } from 'vue';

const otherAlgo = [
    "Execution lags or manual confirmation needed",
    "Limited or DIY-only strategies",
    "Limited or manual-only risk control",
    "Basic or no performance tracking",
    "Requires coding expertise",
    "Complex or outdated UI",
    "Inconsistent security measures",
    "Limited or manual intervention required"
]

const fusion = [
    "Expertly designed, backtested strategies ready for immediate use",
    "Lightning-fast, no delays",
    "Automated stop-loss, take-profit, and position sizing",
    "Detailed P&L, win rates, and drawdown metrics",
    "One-click deployment",
    "Runs continuously, even when offline",
    "Intuitive, easy to navigate",
    "Bank-grade encryption & 99.9% uptime"
]
</script>

<template>
  <section class="max-w-6xl 2xl:max-w-7xl mx-auto py-20 my-16 lg:mt-24 px-4 xl:px-0">
    <div class="text-center">
      <h1 class="font-bold text-[30px] text-white">Why Choose Us Over the Competition?</h1>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 w-full xl:w-[80%] gap-8 mx-auto mt-12">
      <div class="border border-dashed border-[#DE4242] bg-[#DE4242]/15 py-14 px-8 rounded-xl">
        <div class="relative">
          <p class="font-bold text-white text-[32px]">Other Algo</p>
          <div class="">
            <img src="/src/assets/svg/cross.svg" alt="" class="absolute top-[-10px] left-[30px] w-[100px]" />
          </div>
        </div>

        <div class="mt-16">
            <div v-for="item in otherAlgo" class="flex items-center text-white gap-2 mt-8">
            <img src="/src/assets/svg/wrong.svg" alt="" class="w-[25px]">
            <p>{{ item }}</p>
        </div>
        </div>
      </div>


      <div class="border border-dashed border-[#1ADC5B] bg-[#1ADC5B]/15 text-white py-14 px-8 rounded-xl">
        <div class="relative">
          <p class="font-bold text-[32px]">Fusion X</p>
          <div class="">
            <img src="/src/assets/svg/correct.svg" alt="" class="absolute top-[-20px] left-[0px] w-[150px]" />
          </div>
        </div>

        <div  class="mt-16">
            <div v-for="item in fusion" class="flex items-center gap-2 mt-8">
            <img src="/src/assets/svg/right.svg" alt="" class="w-[25px]">
            <p>{{ item }}</p>
        </div>
        </div>
      </div>
    </div>
  </section>
</template>
