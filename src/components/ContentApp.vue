<template>
    <div class="content-app">
      <div class="jumbo-main">

      </div>
      <div class="bg-black">
        <div class="container">
          <div class="row flex-wrap justify-content-between py-5">
            <div class="col-2 d-flex flex-wrap px-2" v-for="(card,index) in comicsArray" :key="index">
              <Card :img="card.thumb" :title="card.series" :alt="card.type"/>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
import {comics} from '../data/dc-comics.js';
import Card from './Card.vue';
    export default {
        name: 'ContentApp',
        components:{
          Card
        },
        data(){
          return{
            comicsArray: comics
          }
        }
    }
</script>

<style lang="scss" >
    .content-app{
      .jumbo-main{
        height: 450px;
        overflow: hidden;
        background-image: url('/images/jumbotron.jpg');
        background-repeat: no-repeat;
        background-position-x: center;
      }
      .bg-black{
        background-color: black;
      }
    }
    h1{
      font-size: 2em;
      font-weight: 700; 
      margin:0
    }
</style>