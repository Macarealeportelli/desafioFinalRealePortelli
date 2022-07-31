<template>
  <div>
    <NavBar/>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
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
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 10px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
