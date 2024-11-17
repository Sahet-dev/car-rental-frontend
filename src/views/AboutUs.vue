<template>
  <div class="min-h-screen bg-gradient-to-br from-gray-50 to-gray-100 py-12">
    <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <div class="text-center mb-12">
        <h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl md:text-6xl">
          <span class="block">About Us</span>
          <span class="block text-blue-600">Our Journey & Mission</span>
        </h1>
        <p class="mt-3 max-w-md mx-auto text-base text-gray-500 sm:text-lg md:mt-5 md:text-xl md:max-w-3xl">
          Learn more about our passion for cars and how we strive to bring the best rides to you
        </p>
      </div>

      <!-- Our Mission Section -->
      <div class="max-w-3xl mx-auto mb-12">
        <div class="bg-white rounded-2xl shadow-xl p-6 space-y-6 sm:space-y-0 sm:flex sm:space-x-4">
          <div class="sm:w-1/2">
            <h2 class="text-2xl font-semibold text-gray-800">Our Mission</h2>
            <p class="mt-3 text-gray-600">
              We aim to provide an unparalleled car rental experience, offering a wide selection of premium vehicles for all types of needs.
              Whether you're looking for a quick getaway or a long road trip, our fleet is equipped to make your journey exceptional.
            </p>
          </div>
          <div class="sm:w-1/2">
            <h2 class="text-2xl font-semibold text-gray-800">Our Values</h2>
            <p class="mt-3 text-gray-600">
              Customer satisfaction is our top priority. We focus on delivering quality service, reliable vehicles, and a seamless booking experience.
              Our team works tirelessly to ensure every customer drives away with a smile.
            </p>
          </div>
        </div>
      </div>

      <!-- Team Section -->
      <div class="max-w-5xl mx-auto mb-12">
        <h2 class="text-3xl font-bold text-center text-gray-800 mb-6">Meet the Team</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Team Member 1 -->
          <div class="text-center bg-white p-6 rounded-lg shadow-lg">
            <img src="https://via.placeholder.com/150" alt="Team Member 1" class="mx-auto rounded-full mb-4" />
            <h3 class="text-xl font-semibold text-gray-800">John Doe</h3>
            <p class="text-gray-500">CEO & Founder</p>
            <p class="mt-2 text-gray-600">
              John is the visionary behind our company, with a passion for cars and customer experience.
            </p>
          </div>
          <!-- Team Member 2 -->
          <div class="text-center bg-white p-6 rounded-lg shadow-lg">
            <img src="https://via.placeholder.com/150" alt="Team Member 2" class="mx-auto rounded-full mb-4" />
            <h3 class="text-xl font-semibold text-gray-800">Jane Smith</h3>
            <p class="text-gray-500">Operations Manager</p>
            <p class="mt-2 text-gray-600">
              Jane oversees the day-to-day operations, ensuring everything runs smoothly and customers receive exceptional service.
            </p>
          </div>
          <!-- Team Member 3 -->
          <div class="text-center bg-white p-6 rounded-lg shadow-lg">
            <img src="https://via.placeholder.com/150" alt="Team Member 3" class="mx-auto rounded-full mb-4" />
            <h3 class="text-xl font-semibold text-gray-800">Alex Johnson</h3>
            <p class="text-gray-500">Customer Relations</p>
            <p class="mt-2 text-gray-600">
              Alex builds strong relationships with our customers, ensuring their satisfaction and loyalty.
            </p>
          </div>
        </div>
      </div>

      <!-- Contact Section -->
      <div class="max-w-3xl mx-auto text-center mb-12">
        <h2 class="text-3xl font-semibold text-gray-800 mb-4">Contact Us</h2>
        <p class="text-lg text-gray-600 mb-4">
          Have questions or need assistance? Feel free to reach out, and we’ll be happy to help!
        </p>
        <a
            href="mailto:contact@carrental.com"
            class="inline-block bg-blue-600 text-white py-3 px-6 rounded-lg hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500">
          Get in Touch
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
// Add any necessary logic here if required for the AboutUs page
</script>

<style scoped>
/* Optional custom styles */
</style>
