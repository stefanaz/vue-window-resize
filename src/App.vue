<template>
  <div id="app">
    <WindowResize v-model="window"/>
  </div>
</template>

<script>
import WindowResize from './components/WindowResize.vue'

export default {
  name: 'App',
  components: {
    WindowResize
  },
  data() {
    return {
      window: {
        width: 0,
        height: 0,
      }
    }
  },
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
