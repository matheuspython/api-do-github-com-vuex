<template>
  <TheHeader />
  <router-view/>
</template>
<script>
import TheHeader from './components/TheHeader.vue';
  export default {
    components: { TheHeader }
}
</script>
<style>
 *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  html, body {
    height: 100%;
    font-family: 'Roboto', 'Open Sans', sans-serif;
  }
  body{
    background-color: #121214;
    color: #fff;
  }
  .container{
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;
    padding: 15px 2%;
  }
  ul{
    list-style: none;
  }
  a{
    color: #fff;
    text-decoration: none;
  }
  ::-webkit-scrollbar {
   width: 8px;
 }
 ::-webkit-scrollbar-thumb {
   background-color: #202225;
   border-radius: 4px;
 }
 ::-webkit-scrollbar-track {
   background-color: #2f3136;
 }
</style>
