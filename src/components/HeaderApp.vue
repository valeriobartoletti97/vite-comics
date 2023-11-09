<template>
  <div>
      <header class="container d-flex justify-content-between">
         <img src="/images/dc-logo.png" alt="logo">
         <ul class="nav d-flex justify-content-between align-items-center flex-nowrap ">
            <li class="nav-item px-3 text-uppercase" v-for="(element,index) in navSections" :key="index">
                <a :class="{'active-section' : element.active=== true}" :href="href">
                    {{ element.text }}
                </a>
            </li>
         </ul>
      </header>
  </div>
</template>

<script>
    export default {
        name: 'HeaderApp',
        data(){
            return{
                navSections: [
                    {
                        text:'Characters',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Comics',
                        href:'#',
                        active: true
                    },
                    {
                        text:'Movies',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Tv',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Games',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Collectibles',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Videos',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Fans',
                        href:'#',
                        active: false
                    },
                    {
                        text:'News',
                        href:'#',
                        active: false
                    },
                    {
                        text:'Shop',
                        href:'#',
                        active: false
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
     header{
        padding:20px 0;
        img{
            width:80px;
        }
        li{
            font-weight: 800;
        }
        a{
            text-decoration: none;
            color:black;
            &:hover{
                cursor: pointer;
            }
        }
        .active-section{
            color: #0282f9;
        }
     }
</style>