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
export default {
  name: 'ModuleTemplate',
  props: {
    moduleCounter: 0,
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
