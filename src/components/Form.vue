<template>
    
      <div class="w-full max-w-md bg-[#23BDB9] rounded-lg p-8 shadow-lg" id="form">
        <h1 class="text-2xl font-bold text-center text-black mb-6">Fill the form</h1>
        
        <form @submit.prevent="submitForm">
          <div class="space-y-4">
            <div>
              <input
                v-model="formData.name"
                type="text"
                placeholder="Your Name"
                class="w-full p-3 rounded-md border-0 focus:ring-2 focus:ring-teal-300 bg-white text-black"
                required
              />
            </div>
            
            <div>
              <input
                v-model="formData.mobile"
                type="tel"
                placeholder="Mobile Number"
                class="w-full p-3 rounded-md border-0 focus:ring-2 focus:ring-teal-300 bg-white text-black"
                required maxlength="10"
              />
            </div>
            
            <div>
              <input
                v-model="formData.email"
                type="email"
                placeholder="Email"
                class="w-full p-3 rounded-md border-0 focus:ring-2 focus:ring-teal-300 bg-white text-black"
                required
              />
            </div>
            
            <div>
              <input
                v-model="formData.city"
                type="text"
                placeholder="City"
                class="w-full p-3 rounded-md border-0 focus:ring-2 focus:ring-teal-300 bg-white text-black"
                required
              />
            </div>
            
            <button
              type="submit"
              class="w-full p-3 bg-slate-900 hover:bg-slate-800 text-[#23BDB9] rounded-md transition-colors duration-300 font-medium"
            >
              Get free demo now
            </button>
          </div>
        </form>
      </div>
    
  </template>
  
  <script setup>
  import { reactive } from 'vue';
  
  const formData = reactive({
    name: '',
    mobile: '',
    email: '',
    city: ''
  });
  
  const submitForm = () => {
    console.log('Form submitted:', formData);
    // Here you would typically make an API call to submit the form data
    alert('Thanks for submitting! We will contact you shortly.');
    
    // Reset form
    formData.name = '';
    formData.mobile = '';
    formData.email = '';
    formData.city = '';
  };
  </script>