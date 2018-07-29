<template>
  <v-app>
    <v-content>
      <ModuleTimer/>
      <ModuleTimer/>
    </v-content>
  </v-app>
</template>

<script>
import ModuleTimer from './components/modules/ModuleTimer.vue';

export default {
  name: 'App',
  components: {
    ModuleTimer,
  },
  data() {
    return {
    };
  },
};
</script>
