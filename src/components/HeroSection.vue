<script setup>
import Form from './Form.vue';

</script>

<template>
  <section class="min-h-[90vh] bg py-8">
    <div class="w-[90%] mx-auto">
      <img src="/src/assets/svg/logo.svg" alt="">
      <div class="w-full flex flex-wrap lg:flex-nowrap gap-2 items-center h-full py-10">
        <div class="w-full lg:w-[50%] flex flex-col gap-8 py-8">
          <div class="border border-white text-white text-[16px] bg-white/20 w-fit px-6 py-2 rounded-full nrml-text">
            <p>❤️Loved by 5k+ Traders</p>
          </div>

          <h2 class=" text-[36px] lg:text-[47px] font-[700] text-white leading-tight">
           <span class="text-[#3CB3B0]">
            100% Automated <br/>
           </span>  Trading – Smarter, Faster, Profitable.
          </h2>

          <p class=" text-[14px] lg:text-[18px] text-white font-[600]">Our Automated Trading Platform Uses Advanced Auto Risk Management System & Strategies to trade trading in Nifty, Banknifty & More.</p>
          <button class=" w-fit rounded-full bg-[#3CB3B0] px-6 py-2 text-[#050811] text-[16px] font-[600]">
            Start Trading Now
          </button>
        </div>
        <div class="w-full lg:w-[50%] flex border justify-end">
          <Form/>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped>
/* Custom glow effect */
.bg-glow {
  background: radial-gradient(circle, rgba(255, 255, 255, 0.3) 0%, rgba(0, 0, 0, 0) 70%);
  filter: blur(80px);
  transform: translate(-50%, -20%);
  animation: glowAnimation 4s ease-in-out infinite alternate;
}

.bg {
  background-image: url('/src/assets/img/hero-bg.png');
  background-position: right;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>