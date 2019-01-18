<template>

  <section class="date-section">
      <h2>Today is..{{ date }}</h2>
  </section>

</template>

<script>
  import Vue from 'vue';

  console.log(Vue)

  window.onload = function () {
    var date = new Vue({
      el: '.date-section',
      data: {
        text: 'Today is..',
        dateDay: new Date().getDate(),
        dateMonth: new Date().getMonth(),
        dateYear: new Date().getFullYear()

      },
      computed: {
        currentDate: function () {
          return this.dateDay + ' ' + this.dateMonth + ' ' + this.dateYear
        }
      }
    });
  };


  export default {
    data() {
      return {
        date: new Date().getDate()
      }
    }
  }
</script>

<style scoped>
  .date-section {
    color: blue;
  }
</style>
