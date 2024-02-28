<template>
  <div class="wrapper">
    <div class="container">
      <header>
        <Header />
      </header>
      <main>
        <TodayWeather />
      </main>
    </div>
  </div>
</template>

<script setup>

import Header from './components/Header.vue';
import TodayWeather from './components/TodayWeather.vue';
import { ref, onMounted } from 'vue';

</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500&display=swap');

.wrapper {
  font-family: 'Poppins', sans-serif;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: #202020;
}

.container {
  width: 75%;
  height: 100%;
  // background: yellow;
  margin: 0 auto;
}
</style>