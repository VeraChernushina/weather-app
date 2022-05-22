<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" name="search-bar" class="search-bar" placeholder="Search..." />
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">Northampton, UK</div>
          <div class="date">Sunday 22 May 2022</div>
        </div>

        <div class="weather-box">
          <div class="temp">9 C</div>
          <div class="weather">Rain</div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    // api_key: '8f00ebd1a5996a984c246f720c4c482d'
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font: 'Montserrat', sans-serif;
}

#app {
  background-image: url('./assets/cold-bg.jpeg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75));
}

.search-box {
  width: 100%;
  margin-bottom: 30px;
}

.search-bar {
  display: block;
  width: 100%;
  padding: 15px;
  color: #313131;
  font-size: 20px;
  appearance: none;
  border: none;
  outline: none;
  background-color: rgba(255,255,255,0.5);
  border-radius: 0 16px 0 16px;
}

.location-box {
  color: #fff;
  font-size: 32px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0,0,0,0.25);
}

.date {
  font-size: 20px;
  font-weight: 300;
  font-style: italic;
  text-align: center;
}

.weather-box {
  text-align: center;
  color: #fff;
  text-shadow: 3px 6px rgba(0,0,0,0.25);
}

.temp {
  display: inline-block;
  padding: 10px 25px;
  font-size: 102px;
  font-weight: 900;
  background-color: rgba(255,255,255,0.25);
  border-radius: 16px;
  margin: 30px 0;
  box-shadow: 3px 6px rgba(0,0,0,0.25);
}

.weather {
  font-size: 48px;
  font-weight: 700;
  font-style: italic;
}
</style>
