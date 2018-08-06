<template lang="pug">
  v-container.moduleInterface(fluid)
    v-layout(column align-center)
      | test
</template>

<script>
import moment from 'moment'

export default {
  name: 'ModuleInterface',
  data () {
    return {
      timer: ''
    }
  },
  methods: {
    update () {
      setInterval(() => {
        this.timer = moment().format('LTS')
      }, 1000)
    }
  },
  created () {
    moment.locale('fr')
    this.timer = moment().format('LTS')
  },
  mounted () {
    this.update()
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
