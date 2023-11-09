<template>
  <div>
      <header class="container d-flex justify-content-between">
         <img src="/images/dc-logo.png" alt="logo">
      </header>
  </div>
</template>

<script>
    export default {
        name: 'HeaderApp',
    }
</script>

<style lang="scss" scoped>
     header{
        padding:20px 0;
        img{
            width:80px;
        }
     }
</style>