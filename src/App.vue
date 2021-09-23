<template>
  <Leaves/>
  <Home/>
  <Projects/>
</template>

<script>
import Home from './components/Home.vue'
import Leaves from './components/Leaves.vue'
import Projects from './components/Projects.vue'

export default {
  name: 'App',
  components: {
    Home,
    Leaves,
    Projects,
  }
}
</script>

<style>
:root {
    --text-color: #e2e2e2;
    --bg-color:#202124;
}
#app {
  font-family: 'Open Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: var(--text-color);
  line-height: 200%;
}
body {
  margin: 0;
  background: var(--bg-color);
}
</style>
