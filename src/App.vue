<template>
  <div id="app">
    <img class="top-header-img" src="./assets/favicon.png">
    <div class="top-header">
      <h1>Just 不吐槽不酥胡</h1>
    </div>
    <Timeline></Timeline>
  </div>
</template>

<script>
import Timeline from './components/Timeline.vue';

export default {
  name: 'app',
  components: {
    Timeline,
  },
}
</script>

<style>
  * {
    border: 0;
    margin: 0;
    padding: 0;
  }

  html {
    height: 100%;
  }

  #app {
    height: inherit;
    display: flex;
    flex-direction: column;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .top-header{
    margin-bottom: 20px;
  }

  .top-header-img {
    width: 70px;
    margin: 0 auto;
  }
</style>
