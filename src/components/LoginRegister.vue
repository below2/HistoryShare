<template>
  <div class="container mt-5">
    <div class="row justify-content-center">
      <div class="col-md-6">
        <!-- Login Form -->
        <div v-if="activeForm === 'login'">
          <h2 class="mb-4">Login</h2>
          <form @submit.prevent="login">
            <div class="mb-3">
              <label for="loginEmail" class="form-label">Email</label>
              <input type="email" class="form-control" id="loginEmail" v-model="loginData.email" required>
            </div>
            <div class="mb-3">
              <label for="loginPassword" class="form-label">Password</label>
              <input type="password" class="form-control" id="loginPassword" v-model="loginData.password" required>
            </div>
            <button type="submit" class="btn btn-primary">Login</button>
          </form>
          <p class="mt-3">
            Don't have an account? <a href="#" @click="switchForm('register')">Register</a>
          </p>
        </div>

        <!-- Register Form -->
        <div v-else>
          <h2 class="mb-4">Register</h2>
          <form @submit.prevent="register">
            <div class="mb-3">
              <label for="registerName" class="form-label">Name</label>
              <input type="text" class="form-control" id="registerName" v-model="registerData.name" required>
            </div>
            <div class="mb-3">
              <label for="registerEmail" class="form-label">Email</label>
              <input type="email" class="form-control" id="registerEmail" v-model="registerData.email" required>
            </div>
            <div class="mb-3">
              <label for="registerPassword" class="form-label">Password</label>
              <input type="password" class="form-control" id="registerPassword" v-model="registerData.password" required>
            </div>
            <button type="submit" class="btn btn-primary">Register</button>
          </form>
          <p class="mt-3">
            Already have an account? <a href="#" @click="switchForm('login')">Login</a>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const activeForm = ref('login');
const loginData = ref({
  email: '',
  password: '',
});

const registerData = ref({
  name: '',
  email: '',
  password: '',
});

const switchForm = (form) => {
  activeForm.value = form;
};

const login = () => {
  // Implement login logic
  console.log('Login:', loginData.value);
};

const register = () => {
  // Implement registration logic
  console.log('Register:', registerData.value);
};
</script>

<style scoped>
/* Add your custom styles here if needed */
</style>
