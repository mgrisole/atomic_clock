<template lang="pug">
  v-container.moduleTimer(fluid)
    v-layout(column align-center)
      | {{timer}}
</template>

<script>
import moment from 'moment';

export default {
  name: 'ModuleTimer',
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
  created() {
    moment.locale('fr');
    this.timer = moment().format('LTS');
  },
  mounted() {
    this.update();
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">

  .moduleTimer
    background-color: #326273
    color: #EEEEEE
    display: flex
    align-items: center

</style>
