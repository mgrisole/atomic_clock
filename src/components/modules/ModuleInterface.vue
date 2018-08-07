<template lang="pug">
  v-container.moduleInterface(fluid)
    v-layout(column align-center)
      | test
</template>

<script>
export default {
  name: 'ModuleInterface',
  props: {
    name: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">

  .moduleInterface
    background-color: #326273
    color: #EEEEEE
    display: flex
    align-items: center

</style>
