<template>
  <main>
    <div>
      <section class="container">
        <h1 class="text-white py-5"> {{ title }} </h1>
      </section>
    </div>
  </main>
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

<style lang="scss" scoped>
    div{
      background-color:black
    }
    h1{
      font-size: 2em;
      font-weight: 700; 
    }
</style>