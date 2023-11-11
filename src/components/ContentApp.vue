<template>
    <div class="bg-black">
      <section class="container">
        <h1 class="text-white py-5"> {{ title }} </h1>
      </section>
    </div>
</template>

<script>
    export default {
        name: 'ContentApp',
        data(){
          return{
            title: '--> Content goes here <--'
          }
        }
    }
</script>

<style lang="scss" >
    .bg-black{
      background-color:black
    }
    h1{
      font-size: 2em;
      font-weight: 700; 
      margin:0
    }
</style>