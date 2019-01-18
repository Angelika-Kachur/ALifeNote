<template>
  <div class="wrapper">

      <AppDate></AppDate>
      <AppGratitudes></AppGratitudes>

    </div>
</template>

<script>
  import Gratitudes from './Gratitudes.vue';
  import Date from './Date.vue';

  export default {
    data() {
      return {

      }
    },
    components: {
      AppGratitudes: Gratitudes,
      AppDate: Date,
    },
    props: {
      /* список переменных для двух компонентов */
    }
  }
</script>

<style> /* no scoped to all css */
  body {
    color: green;
  }
</style>
