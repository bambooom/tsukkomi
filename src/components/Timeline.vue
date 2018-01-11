<template>
  <div class="tsukkomis">
    <div id="timeline">
      <div>
        <Tucao v-for="say in data" :time="say.time" :content="say.content" :emoji="say.emoji" :key="say.time"></Tucao>
      </div>
    </div>
  </div>
</template>

<script>
  import Tucao from './Tucao.vue';

  export default {
    components: {
      Tucao,
    },
    data () {
      return {
        data: require('../../static/data.json')
      };
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .tsukkomis {
    display: flex;
    flex: auto;
    padding: 0rem 1rem 0rem 1rem;
  }

  #timeline {
    position: relative;
    display: table; /* For Firefox */
    height: 100%;
    margin-left: auto;
    margin-right: auto;
    margin-top: 5rem;
    text-align: left;
  }

  #timeline div:after {
    content: '';
    width: 1px;
    position: absolute;
    top: .5rem;
    bottom: 0rem;
    left: 60px;
    z-index: 1;
    background: #c5c5c5;
  }
</style>
