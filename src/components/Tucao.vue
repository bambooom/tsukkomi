<template>
  <section class="year">
    <h3>{{ year }}</h3>
    <section>
      <h4> {{ datetime }} </h4>
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
    },

    computed: {
      year: function () {
        return moment(this.time).year();
      },
      datetime: function () {
        return moment(this.time).format('MMM Do YYYY, h:mm a');
      }
    }
  }
</script>
