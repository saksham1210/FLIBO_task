<template>
  <div id="app">
    <Button/>
  </div>
</template>

<script>
import Button from './components/Button.vue'
export default {
  name: 'App',
  components: {
    Button
  }}
</script>

<style>
#app {

  display:flex;
  align-items: center;
  justify-content: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  height:100vh;
}
</style>
