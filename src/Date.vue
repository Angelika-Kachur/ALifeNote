<template>

  <section class="date-section">
      <h2>Today is..{{ currentDate }}</h2>
  </section>

</template>

<script>
  export default {
    data() {
      return {
        text: 'Today is..',
        dateDay: new Date().getDate(),
        dateMonth: new Date().getMonth(),
        dateYear: new Date().getFullYear()
      }
    },
    computed: {
      currentDate: function () {
        return  this.text + '.' + this.dateDay + '.' + (this.dateMonth + 1) + '.' + this.dateYear
      }
    }
  }
</script>


<style scoped> /* scoped for local css */
  .date-section {
    color: blue;
  }
</style>
