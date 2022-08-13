<template>
  <div class="app">
    <Header></Header>
    <!-- <Main /> -->
    <Content />

  </div>
</template>

<script>
import Header from './views/layout/MainHeader.vue'
import Content from './views/layout/MainContent.vue'
// import Main from './views/MainHome.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    // Main
  }
}
</script>


<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: center;
}
</style>
