<template>
  <div id="app">
    <!-- <equityList/> -->
    <router-view/>
  </div>
</template>

<script>
// import index from './components/index.vue'
// import service from './components/service.vue'
import equityList from './components/equityList.vue'


export default {
  name: 'App',
  components: {
    // index,
    // service,
    equityList
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
  margin-top: 60px;
}
</style>
