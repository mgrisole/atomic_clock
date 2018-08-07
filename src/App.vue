<template lang="pug">
  v-app
    v-content
      ModuleContainer
        ModuleInterface
        ModuleInterface
</template>

<script>
import ModuleContainer from './components/modules/ModuleContainer'
import ModuleTimer from './components/modules/ModuleTimer'
import ModuleWeather from './components/modules/ModuleWeather'
import ModuleInterface from './components/modules/ModuleInterface'

export default {
  name: 'App',
  components: {
    ModuleContainer,
    ModuleTimer,
    ModuleWeather,
    ModuleInterface
  },
  data () {
    return {
    }
  }
}
</script>
