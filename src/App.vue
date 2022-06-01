
<template>

<div id="app">
<main>
  <div class="buscador">
    <input type="text" class="buscadorcito" placeholder="Search..." />
    </div>
    <div class="weather-wrap">
      <div class="location-box">
        <div class="location"> Buenos Aires, Arg</div>
        <div class="date"> Lunes 6 junio 2022</div>
</div>
      <div class="weather-box">
        <div class="temperature">9°c </div>
        <div class="weather">Clear</div>
       </div>
    </div> 
</main>
</div>
</template>




<script>
export default {
  name: 'app',
  data() {
    return {
      api_key: '6a49ff79919f709add61a42ef87a1fca'
    }
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
  font-family: 'roboto';
}
#app {
  background-image: url('./assets/cold.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.5s;
}

main {
  min-height: 100vh;
  padding: 25px;

  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25),rgba(0, 0, 0, 0.75));
}
.buscador {
  width: 100%;
  margin-bottom: 30px;
}
.buscadorcito , .buscador {
  display: block;
  width: 100%;
  padding: 15px;
  color: #313131;
  font-size: 20px;
  appearance: none;
  border: none;
  outline: none;
  background: none;

box-shadow: 0px 0px 15px rgba(0, 0 , 0 ,0.25);
  background-color: rgba(255, 255, 255 0.5);
  border-radius: 0px 15px 0px 15px;
  transition: 0.4s;
}
.buscadorcito , .buscador:focus{
  box-shadow: 0px 0px 15px rgba(0, 0 , 0 ,0.25);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 15px 0px 15px 0px;
}

.location-box .location{
  color: #FFF;
  font-size: 30px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0, 0, 0, 0.25);
}

.location-box .date{
  color: #FFF;
  font-size: 20px;
  font-weight: 300;
  text-align: center;
  font-style: italic;
  
}

.weather-box {
  text-align: center;
}

.weather-box .temperature {
  display: inline-block;
  padding: 10px 25px;
  color: #FFF;
  font-size: 100px;
  font-weight: 900;

  text-shadow: 3px 6px rgba(0, 0 , 0 ,0.25);
  background-color: rgba(255, 255, 255, 0.25);
  border-radius: 16px;
  margin: 30px 0px;

  box-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}

.weather-box .weather{
  color: #FFF;
  font-size: 45px;
  font-weight: 700;
  font-style: italic;
  text-shadow: 3px 6px rgba(0, 0 , 0 ,0.25);
}
</style>
