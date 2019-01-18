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
    }
  }
</script>

<style>
  body {
    color: green;
  }
</style>
