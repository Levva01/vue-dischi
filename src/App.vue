<template>
  <div id="app">

    <BaseHeader/>

  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue'

export default {
  name: 'App',
  components: {
    BaseHeader,
  }
}
</script>

<style lang="scss">

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
