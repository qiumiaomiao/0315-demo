<template>
  <div id="app"> 
    <selects></selects>
  </div>
</template>

<script>
  import Selects from './components/select';
  export default {
    name: 'App',
    components:{Selects}
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
</style>
