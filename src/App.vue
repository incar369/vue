<template>
  <div id="app">
    <Header/>
    <Content/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/h.vue'
import Content from './components/c.vue'
import Footer from './components/f.vue'

export default {
  name: 'App',
  components: {
    Header,Content,Footer
  }
}
</script>

<style>
body{
  margin:0px auto;
}
#app {
  display:block;
  box-sizing: content-box;
  text-align: center;
  min-height: 100%;
  color: #2c3e50;
  margin-top: 0 px auto;
}
</style>
