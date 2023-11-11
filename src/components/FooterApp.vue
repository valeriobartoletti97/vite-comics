<template>
<footer>
  <div class="container d-flex justify-content-between align-items-center align-content-center py-4">
    <button class="text-uppercase py-3">
      <a class="p-3" href="#">Sign-up now!</a>
    </button>
    <div class="d-flex justify-content-between align-items-center flex-nowrap">
      <h4 class="text-uppercase px-2">Follow us</h4>
      <div class="px-2">
        <img src="/images/footer-facebook.png" alt="#">
      </div>
      <div class="px-2">
        <img src="/images/footer-periscope.png" alt="#">
      </div>
      <div class="px-2">
        <img src="/images/footer-pinterest.png" alt="#">
      </div>
      <div class="px-2">
        <img src="/images/footer-twitter.png" alt="#">
      </div>
      <div class="px-2">
        <img src="/images/footer-youtube.png" alt="#">
      </div>
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
      h4{
        font-size: 1.4em;
        color: $primary-color;
        font-weight: 800;
        margin: 0 !important;
      }
      div{
        img{
          width:30px;
          display: block;
          
        }
      }
    }
</style>