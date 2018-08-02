<template lang="pug">
  v-container.moduleContainer(fluid)
    v-slide-y-transition(mode="out-in")
      v-layout(column align-center)
        slot
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
