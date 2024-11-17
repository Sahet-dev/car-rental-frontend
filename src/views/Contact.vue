<template>
  <div class="min-h-screen bg-gradient-to-br from-gray-50 to-gray-100 py-12">
    <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <div class="text-center mb-12">
        <h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl md:text-6xl">
          <span class="block">Get in Touch</span>
          <span class="block text-blue-600">We're Here to Help</span>
        </h1>
        <p class="mt-3 max-w-md mx-auto text-base text-gray-500 sm:text-lg md:mt-5 md:text-xl md:max-w-3xl">
          Have any questions or need assistance? Reach out to us today.
        </p>
      </div>

      <!-- Contact Form Section -->
      <div class="max-w-3xl mx-auto mb-12">
        <div class="bg-white rounded-2xl shadow-xl p-6 space-y-6">
          <!-- Name Input -->
          <div>
            <label for="name" class="block text-sm font-medium text-gray-700">Full Name</label>
            <input
                id="name"
                v-model="name"
                type="text"
                placeholder="Your Full Name"
                class="block w-full mt-2 p-3 border border-gray-200 rounded-xl text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
          </div>

          <!-- Email Input -->
          <div>
            <label for="email" class="block text-sm font-medium text-gray-700">Email Address</label>
            <input
                id="email"
                v-model="email"
                type="email"
                placeholder="Your Email Address"
                class="block w-full mt-2 p-3 border border-gray-200 rounded-xl text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
          </div>

          <!-- Message Textarea -->
          <div>
            <label for="message" class="block text-sm font-medium text-gray-700">Message</label>
            <textarea
                id="message"
                v-model="message"
                placeholder="Your Message"
                rows="4"
                class="block w-full mt-2 p-3 border border-gray-200 rounded-xl text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-500"
            ></textarea>
          </div>

          <!-- Submit Button -->
          <div>
            <button
                @click="submitForm"
                class="w-full py-3 px-6 bg-blue-600 text-white rounded-xl shadow-md hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500 transition duration-200"
            >
              Send Message
            </button>
          </div>
        </div>
      </div>

      <!-- Thank You Message -->
      <div v-if="submitted" class="text-center py-12">
        <div class="text-gray-400 mb-4">
          <svg class="mx-auto h-12 w-12" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 0v4m0-4h4m-4 0h-4" />
          </svg>
        </div>
        <h3 class="text-lg font-medium text-gray-900 mb-2">Message Sent</h3>
        <p class="text-gray-500">Thank you for reaching out! We'll get back to you soon.</p>
      </div>

      <!-- Empty State for No Message Sent -->
      <div v-if="!submitted" class="text-center py-12">
        <div class="text-gray-400 mb-4">
          <svg class="mx-auto h-12 w-12" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
          </svg>
        </div>
        <h3 class="text-lg font-medium text-gray-900 mb-2">We'd Love to Hear From You</h3>
        <p class="text-gray-500">Fill out the form and send us your message, and we will respond as soon as possible.</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const name = ref('');
const email = ref('');
const message = ref('');
const submitted = ref(false);

const submitForm = () => {
  if (name.value && email.value && message.value) {
    // Process the form data (for example, sending it to a server)
    submitted.value = true;
  } else {
    alert('Please fill in all the fields');
  }
};
</script>

<style scoped>
/* Optional additional styles for customization */
</style>
