<template>
  <Home/>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
:root {
    --text-color: #e2e2e2;
    --bg-color:#202124;
}
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: var(--text-color);
}
body {
  margin: 0;
  background: var(--bg-color);
}
</style>
