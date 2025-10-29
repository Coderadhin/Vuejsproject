<template>
  <div class='home'>
    <img src='/New.png' class='bg' alt='Background' />
    <div class='overlay'>
      <button @click='listenStory'>Let's Read</button>
    </div>
  </div>
</template>

<script setup>
function listenStory() {
  alert('Audio feature coming soon!')
}
</script>

<style scoped>
.home {
  position: relative;
  width: 100%;
  height: 100vh;
}

.bg {
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(0.85);
}

.overlay {
  position: absolute;
  top: 10%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #4B0082;
}

button {
  background-color: #cccccc;
  border: none;
  padding: 0.75rem 1.5rem;
  border-radius: 1rem;
  font-size: 1.1rem;
  cursor: pointer;
}
</style>
