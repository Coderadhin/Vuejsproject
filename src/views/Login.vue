<template>
  <div class='container'>
    <img src='/logo.png' alt='Logo' class='logo' />
    <h2>Login</h2>
    <input type='text' placeholder='Username' v-model='username' />
    <input type='password' placeholder='Password' v-model='password' />
    <button @click='login'>Login</button>
    <a href='#'>Forgot Password?</a>
    <a href='#'>Create Account</a>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router'
import { ref } from 'vue'

const router = useRouter()
const username = ref('')
const password = ref('')

function login() {
  router.push('/home')
}
</script>
