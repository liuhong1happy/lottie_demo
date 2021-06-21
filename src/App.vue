<template>
  <div id="app">
    <lottie v-if="defaultOptions" :width="400" :height="400" :options="defaultOptions" @animCreated="handleCreatedAnimation"/>
  </div>
</template>

<script>
import Lottie from './components/Lottie.vue'

export default {
  name: 'App',
  components: {
    Lottie
  },
  data() {
    return {
      defaultOptions: {
        loop: true,
        path: '/demo.json'
      }
    }
  },
  methods: {
    handleCreatedAnimation: function(anim) {
      console.log(anim)
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
