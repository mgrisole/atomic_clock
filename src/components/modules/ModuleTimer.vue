<template>
  <v-container fluid class="moduleTimer">
    <v-slide-y-transition mode="out-in">
      <v-layout column align-center>
        {{timer}}
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>

<script>
import moment from 'moment';
import ModuleTemplate from './ModuleTemplate.vue';

export default {
  name: 'ModuleTimer',
  extends: ModuleTemplate,
  data() {
    return {
      timer: '',
    };
  },
  methods: {
    update() {
      setInterval(() => {
        this.timer = moment().format('LTS');
      }, 1000);
    },
  },
  mounted() {
    moment.locale('fr');
    this.update();
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.moduleTimer {
  height: calc(100vh/2);
  background-color: #326273;
  color: #EEEEEE;
  display: flex;
  align-items: center;
}
</style>
