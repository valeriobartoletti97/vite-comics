<template>
<footer>
  <div class="container d-flex justify-content-between flex py-4">
    <button class="text-uppercase py-3">
      <a class="p-3" href="#">Sign-up now!</a>
    </button>
    <div class="d-flex justify-content-between">
      <h4 class="text-uppercase">Follow us</h4>
    </div>
  </div>
</footer>
</template>

<script>
    export default {
        name: 'FooterApp',
    }
</script>

<style lang="scss">
@use '../assets/partials/variables' as *;
    footer{
      background-color: $secondary-color;
      button{
        background-color: $secondary-color;
        border: 2px solid $primary-color;
      }
    }
</style>