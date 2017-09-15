<template>
  <div class="top-header">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'header',
  data () {
    return {
      msg: 'Just 不吐槽不酥胡',
    };
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  .top-header{
    margin-bottom: 20px;
  }

/*ul {*/
  /*list-style-type: none;*/
  /*padding: 0;*/
/*}*/

/*li {*/
  /*display: inline-block;*/
  /*margin: 0 10px;*/
/*}*/

a {
  color: #42b983;
}
</style>
