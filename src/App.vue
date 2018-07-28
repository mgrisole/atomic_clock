<template>
  <v-app>
    <v-content>
      <ModuleTimer/>
      <ModuleTimer/>
    </v-content>
  </v-app>
</template>

<script>
import ModuleTimer from './components/ModuleTimer.vue';

export default {
  name: 'App',
  components: {
    ModuleTimer,
  },
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [{
        icon: 'bubble_chart',
        title: 'Inspire',
      }],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    };
  },
};
</script>
