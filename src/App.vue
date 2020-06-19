<template>
  <div id="app">
    <Header/>
    <router-link to="/">Lista</router-link>
    <router-link to="/detail">Detalle</router-link>
    <!--<Detail/>-->
    <router-view></router-view>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
//import Detail from './components/Detail'
import Header from './components/Header'
export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

