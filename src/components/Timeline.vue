<template>
  <div class="tsukkomis">
    <div id="timeline">
      <div>
        <Tucao time="2017-08-29T16:24:00" content="hehhhehhehhehh"></Tucao>
        <section class="year">
          <h3>2016</h3>
          <section>
            <h4> August 17th 8:25pm @ BJ</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
          <section>
            <h4> ?????</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2015</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2014</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2013</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2012</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2011</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2010</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2009</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
        <section class="year">
          <h3>2008</h3>
          <section>
            <h4>August</h4>
            <ul>
              <li>AAAAA</li>
              <li>BBBBB</li>
            </ul>
          </section>
        </section>
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
        msg: 'Just 不吐槽不酥胡',
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

  #timeline h3 {
    position: -webkit-sticky;
    position: sticky;
    top: 5rem;
    color: #888;
    margin: 0;
    font-size: 1em;
    font-weight: 400;
  }

  #timeline section.year {
    position: relative;
    min-width: 400px;
  }

  #timeline section.year:first-child section {
    margin-top: -1.3em;
    /*padding-bottom: 0px;*/
  }

  #timeline section.year section{
    position: relative;
    padding-bottom: 1.25em;
    margin-bottom: 2.2em;
    word-wrap: break-word;
  }

  #timeline section.year section h4 {
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
  #timeline section.year section ul {
    list-style-type: none;
    padding: 0 0 0 75px;
    margin: -1.35rem 0 1em;
    max-width: 32rem;
    font-size: 1em;
  }
  #timeline section.year section ul:last-child {
    margin-bottom: 0;
  }
  #timeline section.year section ul:first-of-type:after {
    content: '';
    width: 10px;
    height: 10px;
    background: #c5c5c5;
    border: 2px solid #fff;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    -ms-border-radius: 50%;
    border-radius: 50%;
    position: absolute;
    left: 54px;
    top: 3px;
    z-index: 2;
  }
  #timeline section.year section ul li {
    margin-left: .5rem;
  }
  #timeline section.year section ul li:before {
    content: '❡';
    margin-left: -.5rem;
    padding-right: .3rem;
  }
  #timeline section.year section ul li:not(:first-child){
    margin-top: .4rem;
  }

  a {
    color: #42b983;
  }
</style>
