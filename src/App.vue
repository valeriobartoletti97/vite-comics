<template>
  <HeaderApp />
  <main>
    <ContentApp />
    <JumboApp />
    <MerchApp />
  </main>
  <FooterApp />
</template>

<script>
  import HeaderApp from './components/HeaderApp.vue';
  import ContentApp from './components/ContentApp.vue';
  import FooterApp from './components/FooterApp.vue';
  import MerchApp from './components/MerchApp.vue';
  import JumboApp from './components/JumboApp.vue';
  export default {
    name:'App',
    components:{
      HeaderApp,
      ContentApp,
      FooterApp,
      MerchApp,
      JumboApp,
    },
    data(){

    },
    methods:{

    }
  }
</script>

<style lang="scss">

</style>