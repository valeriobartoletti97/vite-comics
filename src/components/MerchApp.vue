<template>
    <div class="bg-primary">
        <div class="container">
            <ul class="nav d-flex justify-content-between align-items-center flex-nowrap ">
                <li class="nav-item px-3 text-uppercase" v-for="(element,index) in merch" :key="index">
                    <div>
                        <img :src="element.img" alt="merch-logo">
                        <a :class="{'active-section' : element.active=== true}" :href="href">
                            {{ element.text }}
                        </a>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name:'MerchApp',
        data(){
            return{
                merch: [
                    {
                        img: '/images/buy-comics-digital-comics.png',
                        text: 'Digital Comics',
                        href: '#',
                    },
                    {
                        img: '/images/buy-comics-merchandise.png',
                        text: 'Dc Merchandise',
                        href: '#',
                    },
                    {
                        img: '/images/buy-comics-subscriptions.png',
                        text: 'Subscription',
                        href: '#',
                    },
                    {
                        img: '/images/buy-comics-shop-locator.png',
                        text: 'Comic Shop Locator',
                        href: '#',
                    },
                    {
                        img: '/images/buy-dc-power-visa.svg',
                        text: 'Dc Power Visa',
                        href: '#',
                    },
                ]
            }
        }
    }
</script>

<style lang="scss">
    .bg-primary{
        background-color: #0282f9;
    }
    li , a{
        color:white
    }
    img{
        width: 70px;
    }
</style>