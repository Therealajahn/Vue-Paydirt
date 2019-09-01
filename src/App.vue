<template>
  
  <div id="app">
  
    <IntroPage />
  </div>
</template>

<script>
import IntroPage from "./components/IntroPage.vue";

export default {
  name: 'app',
  components: {
    IntroPage
  },
  
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Lalezar&display=swap');
body{
    background-color: #2989D6;
    margin: 0;
    padding: 0;
}
</style>
