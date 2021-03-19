<template>
  <navbar-lol></navbar-lol>
  <div id="app">
    <Champions :champions="[
    {id: '1', name: 'Garen', role:'Toplaner'},
    {id: '2', name: 'Darius', role:'Toplaner'},
    {id: '3', name: 'Sett', role:'Toplaner'},
    {id: '4', name: 'Irelia', role:'Toplaner'},
    {id: '5', name: 'Malphite', role:'Toplaner'},
    {id: '6', name: 'Mordekaiser', role:'Toplaner'},
    {id: '7', name: 'Jax', role:'Toplaner'},
    {id: '8', name: 'Tryndamere', role:'Toplaner'},
    {id: '9', name: 'Olaf', role:'Toplaner'},
    {id: '10', name: 'Aatrox', role:'Toplaner'},
    ]"/>
  </div>
</template>

<script>

import NavbarLol from './components/NavbarLol.vue'
import Champions from './components/Champions.vue'

export default {
  name: 'App',
  components: {
    NavbarLol,
    Champions
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
}
</style>
