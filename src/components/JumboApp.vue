<template>
        <div class="jumbo-main">
            <div class="container">
                <div class="row justify-content-between">
                    <div class="col-6 d-flex">
                        <div class="pe-4 d-flex flex-column">
                            <h3 class="text-uppercase pt-5 pb-3">Dc comics</h3>
                            <ul>
                                <li class="d-flex flex-column" v-for="(link,index) in linksComics" :key="index">
                                    <a class="pt-1 link-color" :href="link.href">{{ link.title }}</a>
                                </li>
                            </ul>
                            <h3 class="text-uppercase pt-2 pb-3">Shop</h3>
                            <ul>
                                <li class="d-flex flex-column" v-for="(link,index) in linksShop" :key="index">
                                    <a class="pt-1 link-color" :href="link.href">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="pe-4 d-flex flex-column">
                            <h3 class="text-uppercase pt-5 pb-3">Dc</h3>
                            <ul>
                                <li class="d-flex flex-column" v-for="(link,index) in linksDc" :key="index">
                                    <a class="pt-1 link-color" :href="link.href">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="d-flex flex-column">
                            <h3 class="text-uppercase pt-5 pb-3">Sites</h3>
                            <ul>
                                <li class="d-flex flex-column" v-for="(link,index) in linksSites" :key="index">
                                    <a class="pt-1 link-color" :href="link.href">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-6">
                        <img class="bg-logo" src="/images/dc-logo-bg.png" alt="dc logo">
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
    export default {
        name:'JumboApp',
        data(){
            return{
                linksComics: [
                    {
                        title: 'Characters',
                        href: '#'
                    },
                    {
                        title: 'Comics',
                        href: '#'
                    },
                    {
                        title: 'Movies',
                        href: '#'
                    },
                    {
                        title: 'TV',
                        href: '#'
                    },
                    {
                        title: 'Games',
                        href: '#'
                    },
                    {
                        title: 'News',
                        href: '#'
                    },
                    {
                        title: 'Characters',
                        href: '#'
                    },
                ],
                linksDc: [
                    {
                        title: 'Terms Of Use',
                        href: '#',
                    },
                    {
                        title: 'Privacy Policy (New)',
                        href: '#',
                    },
                    {
                        title: 'Ad Choices',
                        href: '#',
                    },
                    {
                        title: 'Advertising',
                        href: '#',
                    },
                    {
                        title: 'Jobs',
                        href: '#',
                    },
                    {
                        title: 'Subscriptions',
                        href: '#',
                    },
                    {
                        title: 'Talent Workshops',
                        href: '#',
                    },
                    {
                        title: 'CPSC Certificates',
                        href: '#',
                    },
                    {
                        title: 'Ratings',
                        href: '#',
                    },
                    {
                        title: 'Shop Help',
                        href: '#',
                    },
                    {
                        title: 'Contact Us',
                        href: '#',
                    },
                ],
                linksSites: [
                    {
                        title: 'DC',
                        href: '#'
                    },
                    {
                        title: 'MAD Magazine',
                        href: '#'
                    },
                    {
                        title: 'DC Kids',
                        href: '#'
                    },
                    {
                        title: 'DC Universe',
                        href: '#'
                    },
                    {
                        title: 'DC Power Visa',
                        href: '#'
                    },
                ],
                linksShop:[
                    {
                        title: 'Shop DC',
                        href: '#'
                    },
                    {
                        title: 'Shop DC Collectibles',
                        href: '#'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss">
     .jumbo-main{
        background-image: url('/images/footer-bg.jpg');
        color: white;
        overflow: hidden;
     }
     .bg-logo{
        width: 500px;
     }
     h3{
        font-size: 1.5em;
        font-weight: 800;
     }
     .link-color{
        color:gray;
     }
</style>