<template lang="pug">
  v-container.moduleWeahter(fluid)
    v-layout(column align-center)
      | {{weather}}
</template>

<script>
import openWeather from 'openweather-apis';

export default {
  name: 'ModuleWeather',
  data() {
    return {
      weather: '',
      metric: '',
    };
  },
  mounted() {
    openWeather.setLang('fr');
    openWeather.setCity('Toulouse');
    openWeather.setAPPID('e169fc4be7c5b637dd06aa4f62fc88dd');
    openWeather.getTemperature((err, temp) => {
      this.weather = temp;
    });
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">

  .moduleWeahter
    background-color: #326273
    color: #EEEEEE
    display: flex
    align-items: center

</style>
