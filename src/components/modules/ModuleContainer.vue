<template>
  <v-container fluid class="moduleContainer">
    <v-slide-y-transition mode="out-in">
      <v-layout column align-center>
        <slot/>
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>

<script>
export default {
  name: 'ModuleContainer',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">

  .moduleContainer
    height: 100vh
    display: flex

</style>
