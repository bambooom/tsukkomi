<template>
  <section class="tucao">
    <h3 class="tucao-emoji">{{ emoji }}</h3>
    <section>
      <h4 class="tucao-time"> {{ datetime }} </h4>
      <ul>
        <li>{{ content }}</li>
      </ul>
    </section>
  </section>
</template>

<script>
  import moment from 'moment';

  export default {
    props: {
      time: String,
      content: String,
      emoji: String,
    },

    computed: {
      datetime: function () {
        return moment(this.time).format('MMM Do YYYY, h:mm a');
      }
    }
  }
</script>

<style>
  .tucao {
    position: relative;
    min-width: 400px;
  }

  .tucao section{
    position: relative;
    padding-bottom: 1.25em;
    margin-bottom: 2.2em;
    word-wrap: break-word;
  }

  .tucao .tucao-time {
    position: absolute;
    bottom: 0;
    right: 0;
    font-size: .9em;
    font-weight: 400;
    line-height: 1.2em;
    margin: 0;
    /*padding: 0 0 0 89px;*/
    color: #c5c5c5;
  }
  .tucao section ul {
    list-style-type: none;
    padding: 0 0 0 75px;
    margin: -1.35rem 0 1em;
    max-width: 32rem;
    font-size: 1em;
  }
  .tucao section ul:last-child {
    margin-bottom: 0;
  }
  .tucao section ul:first-of-type:after {
    content: '';
    width: 10px;
    height: 10px;
    background: #c5c5c5;
    border: 2px solid #fff;
    border-radius: 50%;
    position: absolute;
    left: 54px;
    top: 3px;
    z-index: 2;
  }
  .tucao section ul li {
    margin-left: .5rem;
  }
  .tucao section ul li:before {
    content: '';
    margin-left: -.5rem;
    padding-right: .3rem;
  }
</style>
