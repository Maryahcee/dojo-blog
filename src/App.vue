<template>
  <div >
    <router-link to="/">Home</router-link> 
  </div>
  <router-view/>
</template>

<script>

export default {
  name: 'Home',
  setup() {
    
  },
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
