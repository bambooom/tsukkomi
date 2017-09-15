<template>
  <div id="app">
    <h1>💁🏼</h1>
    <Top></Top>
    <Timeline></Timeline>
  </div>
</template>

<script>
import Top from './components/Top.vue';
import Timeline from './components/Timeline.vue';

export default {
  name: 'app',
  components: {
    Top,
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
</style>
