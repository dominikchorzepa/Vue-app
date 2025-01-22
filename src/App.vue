<template>
  <MenuGlowne />
</template>

<script>
import MenuGlowne from './components/MenuGlowne.vue';

export default {
  name: 'App',
  components: { MenuGlowne }
}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  color: #2c3e50;
}
body{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: #f1f4f0;
}
</style>
