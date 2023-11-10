<template>
    <footer>
        <div class="bg-img">
            <div class="container top-footer" v-for="(link, index) in actionLinks" :key = 'index'>
                <h4>{{ link.title }}</h4>
                <ul>
                    <li v-for="(links, index) in link.links" :key="index"><a href="#">{{ link.links }}</a></li>
                </ul>
            </div> 
        </div>
        <div>
            <div class="container bottom-footer">
                <button type="button" class="btn btn-secondary btn-lg mt-3">SIGN UP</button>
            </div> 
            <div>
                <span><strong>FOLLOW US</strong></span>
                <img v-for="img in mediaLogos" :src="mediaLogos.social" alt="">
            </div>
        </div>
    </footer>
</template>
  
<script>
    export default {
        name: 'AppFooter',
        data(){
            return{
                actionLinks:[
                    {
                        title:  'DC COMICS',
                        links: [
                            [
                                'Characters',
                                'Comics',
                                'Movies',
                                'TV',
                                'Games',
                                'Videos',
                                'News' 
                            ],
                        ]
                    },
                    {
                        title:  'SHOP',
                        links: [
                            [
                                'Shop DC',
                                'Shop DC Collectibles'
                            ],
                        ]
                    },
                    {
                        title:  'DC',
                        links: [
                            [
                                'Terms Of Use',
                                'Privacy policy (New)',
                                'Ad Choices',
                                'Advertising',
                                'Jobs',
                                'Subscriptions',
                                'Talent Workshops',
                                'CPSC Certifictes',
                                'Ratings',
                                'Shop Help',
                                'Contact Us'
                            ],
                        ]
                    },
                    {
                        title:  'SITES',
                        links: [
                            [
                                'DC',
                                'MAD Magazine',
                                'DC Kids',
                                'DC Universe',
                                'DC Power Visa' 
                            ],
                        ]
                    },
                ],
                mediaLogos: [
                    {
                        social: '/public/img/footer-facebook.png',
                    },
                    {
                        social: '/public/img/footer-periscope.png',
                    },
                    {
                        social: '/public/img/footer-pinterest.png',
                    },
                    {
                        social: '/public/img/footer-twitter.png',
                    },
                    {
                        social: '/public/img/footer-youtube.png',
                    }
                 ]   
            }
        },
        methods:{

        }
       
    };
    
</script>
  
<style lang="scss" scoped>
  .bg-img{
    height: 450px;
    background-image: url('/public/img/footer-bg.jpg');
  }
</style>