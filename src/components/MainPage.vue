<template>
  <div class="main-page" id="MainPage">
    <h1 class="heading-name">{{info.name}}</h1>
    <div>
      <div></div>
      <div>
        <img src="" alt="">
      </div>
      <div>
        <ul>
          <li><a href=""><i class="fab fa-instagram"></i></a></li>
          <li><a href=""><i class="fab fa-twitter"></i></a></li>
          <li><a href=""><i class="fab fa-facebook-f"></i></a></li>
          <li><a href=""><i class="fas fa-envelope-square"></i></a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import axios from 'axios'
import VueAxios from 'vue-axios'
Vue.use(VueAxios, axios)

export default {
  name:"MainPage",
  data(){
    return {info:null}
  },
  mounted()
  {
    Vue.axios.get("https://hirng-x2021.glitch.me/api")
    .then(response => {
      this.info = response.data
    })
  }
}
</script>

<style>
  .heading-name{
    margin: 0 auto;
  }
</style>