<template>
    <div class="relative w-[90%] mx-auto bg-[#0703120F] rounded-xl overflow-hidden shadow-2xl">
      <!-- Inner shadow effect -->
      <div class="absolute inset-0 shadow-inner pointer-events-none border border-teal-500/20 rounded-xl"></div>
      
      <div class="flex flex-col justify-between md:flex-row pt-8 md:pt-12">
        <!-- Left content -->
        <div class="w-full md:w-2/5 flex flex-col justify-center px-8">
          <h2 class="text-[32px] font-[700] text-white mb-4">Connect Your Favorite Broker</h2>
          <p class="text-white mb-8 text-[19.2px] font-[600]">
            Our platform integrates with leading brokers, allowing you to trade seamlessly.
          </p>
          <div>
            <a href="#form" class="bg-[#3CB3B0] text-[#040810] font-[700] text-[16px] py-3 px-6 rounded-full transition duration-300">
              Get free demo now
            </a>
          </div>
        </div>
        
        <!-- Right content - placeholder for the trading interface image -->
        <div class="w-full md:w-3/5 flex justify-end mt-8 md:mt-0">
            <img src="/src/assets/img/connect-bg.png" class=" w-[90%] lg:w-[70%] " alt="" >
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  // Component logic can be added here if needed
  </script>
  
  <style scoped>
  /* Additional custom styles if needed */
  .shadow-inner {
    box-shadow: inset 0 0 100px rgba(0, 0, 0, 0.5), 
                inset 0 0 50px rgba(20, 184, 166, 0.3);
  }
  </style>