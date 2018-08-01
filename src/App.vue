<template>
  <v-app>
    <v-content>
      <ModuleContainer>
        <ModuleTimer/>
        <ModuleWeather/>
      </ModuleContainer>
    </v-content>
  </v-app>
</template>

<script>
import ModuleContainer from './components/modules/ModuleContainer.vue';
import ModuleTimer from './components/modules/ModuleTimer.vue';
import ModuleWeather from './components/modules/ModuleWeather.vue';

export default {
  name: 'App',
  components: {
    ModuleContainer,
    ModuleTimer,
    ModuleWeather,
  },
  data() {
    return {
    };
  },
};
</script>
