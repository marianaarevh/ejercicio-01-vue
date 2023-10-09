<template>
  <div id="app">
    <MenuPrincipal/>
    <LandingPage />
    <EnlaceVbind url="https://vuejs.org"/>
  </div>
</template>

<script>
import MenuPrincipal from './components/MenuPrincipal.vue'
import LandingPage from './components/LandingPage.vue'
import EnlaceVbind from './components/EnlaceVbind.vue'


export default {
  name: 'App',
  components: {
    MenuPrincipal,
    LandingPage,
    EnlaceVbind
    
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
  margin-top: 0px;
}
</style>
