<template>
  <div id="app">
   <MainPage/>
  </div>
</template>

<script>
import MainPage from './components/MainPage.vue'
export default {
  name: 'app',
  components: {
    MainPage
  }
}
</script>

<style>
body{
  background: linear-gradient(to right, #c20049 50%, #d10061 50% 100%);
  color: white;
  font-family: 'Roboto', sans-serif;
  font-weight: 100;
}
#app { 
  background-size: cover;
}
</style>
