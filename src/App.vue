<template>
  <div id="app">
    <my_web_sidebar></my_web_sidebar>
    <my_web_header></my_web_header>
    <my_web_content></my_web_content>
    <intro></intro>
  </div>
</template>

<script>

  import intro from './components/intro.vue'
  import my_web_content from './components/my_web_content.vue'
  import my_web_header from './components/my_web_header.vue'
  import my_web_sidebar from './components/my_web_sidebar.vue'
  // eslint-disable-next-line
  import Vuetify from 'vuetify'

  export default {
    name: 'app',
    components: {
      intro,
      my_web_content,
      my_web_header,
      my_web_sidebar,
      // eslint-disable-next-line
      Vuetify
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  my_web_content {
    z-index: 0;
  }

  body {
    margin: 0;
    padding-top: 5%;
    background-image: './assets/background.jpg';
  }
  html { 
  background: url('./assets/background.jpg') no-repeat center center fixed; 
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
</style>