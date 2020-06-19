<template>
  <div id="app">
    <Header/>
    <!--<Detail/>-->
    <List/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import List from './components/List'
import Header from './components/Header'
//import Detail from './components/Detail'
export default {
  name: 'App',
  components: {
    //HelloWorld
    List,
    Header
    //Detail
  }
}
</script>

