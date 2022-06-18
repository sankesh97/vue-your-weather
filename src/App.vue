<script setup>
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div>
    <div className="section container text-center" id="1">
      <div className="row">
        <div className="col-sm-6 p-5">
          <img src="{yourWeatherLogo}" alt="Rain" className="img-fluid" />
        </div>
        <div className="col-sm-6 d-flex flex-column justify-content-center">
          <!----<WeatherInput btnclick={(ele) => onLoading(ele)}></WeatherInput>-->
        </div>
      </div>
    </div>
    <div className="section container text-center" id="2">
      <div className="row">
        <div
          className="col-sm-6 d-flex justify-content-center align-items-center p-5"
        >
          {weather_icon_out}
        </div>
        <div className="col-sm-6">
          <div className="d-flex justify-content-center p-5">{weather_out}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.section {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.main-btn {
  border: none;
  border-top-left-radius: 0;
  border-bottom-left-radius: 0;
  background-color: teal;
}

.main-btn:hover {
  background-color: #505050;
  color: #fff;
}
</style>
