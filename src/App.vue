<template>
  <div class="wrapper">
      <div class="date">
          Today is <span class="date-today">22.12.2018</span>
      </div>

      <section class="gratitude-section">
          <h2>Tell Thanks..{{ message }}</h2>

          <form class="gratitudes">
              <textarea name="gratitude" id="" cols="30" rows="10"></textarea>
              <button class="create-gratitude">Tell one more Thanks</button>
          </form>

          <div class="all-gratitudes">
              <h3> Here are all your gratitudes.</h3>
          </div>
      </section>

    </div>
</template>

<script>
  export default {
    data() {
      return {
        message: 'Hello'
      }
    }
  }
</script>

<style>
  .wrapper {
    padding: 10px;
  }
</style>