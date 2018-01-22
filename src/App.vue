<template>
  <div id="app">
    <div>
    <v-digital-clock timezone="Etc/UTC" city="UTC"/>
    </div>
    <div>
    <v-digital-clock timezone="Asia/Manila" city="Manila"/>
    </div>
    <div>
    <v-digital-clock timezone="America/Los_Angeles" city="PST"/>
    </div>
    <div>
    <v-digital-clock timezone="Europe/London" city="London"/>
    </div>
    <div>
    <v-digital-clock timezone="Europe/Moscow" city="Moscow"/>
    </div>
  </div>
</template>

<script>
import VDigitalClock from './components/VDigitalClock'

export default {
  name: 'App',
  components: {
    VDigitalClock
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
