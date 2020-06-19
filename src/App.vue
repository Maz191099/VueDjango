<template>
  <div id="app">
    <Header/>
    <Categories/>
    <Types/>
    <!--<Detail/>-->
    <router-view></router-view>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
//import Detail from './components/Detail'
import Header from './components/Header'
import Categories from './components/Categories'

import Types from './components/Types'
export default {
  name: 'App',
  components: {
    Header, 
    Categories,
    Types
  }
}
</script>

