<template>
  <div class="not-found">
    <h1>404 - Page Not Found</h1>
    <p>The page you are looking for does not exist or has been moved.</p>
    <button @click="goBackHome">Go Back Home</button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const goBackHome = () => {
  router.push('/'); // Redirect to the home page
};
</script>

<style scoped>
.not-found {
  text-align: center;
  padding: 50px;
}

.not-found h1 {
  font-size: 3em;
  margin-bottom: 20px;
}

.not-found p {
  font-size: 1.2em;
  margin-bottom: 30px;
}

button {
  padding: 10px 20px;
  font-size: 1em;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}
</style>
