<template>
  <div>
    <NavBar/>
    <router-view/>
  </div>
</template>

<script>
import NavBar from '../src/components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
  }
}

</script>
<style>

@import url('https://fonts.googleapis.com/css2?family=Comfortaa&display=swap');

* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Comfortaa', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
