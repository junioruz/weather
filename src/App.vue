<template>
  <div class="wrapper">
    <div class="container">
      <header>
        <Header />
      </header>
      <main>
        <TodayWeather @cityClickName="cityClick" />
      </main>
    </div>
  </div>
</template>

<script setup>

import Header from './components/Header.vue';
import TodayWeather from './components/TodayWeather.vue';

import axios from 'axios';
import { ref, onMounted } from 'vue';

const city = ref('');

const cityClick = (val) => {
  city.value = val;
}

const cityWeather = ref([]);

const getWeather = async () => {
  
  let res = await axios.get('https://api.openweathermap.org/data/2.5/forecast?q=`${city.value}`&appid=9dd86907fe501cec50da3d087e4e9dc09dd86907fe501cec50da3d087e4e9dc0');
  cityWeather.value = [...res.data];


}

onMounted(() => {
  getWeather()
})

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