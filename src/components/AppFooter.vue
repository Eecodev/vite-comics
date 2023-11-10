<template>
    <footer>
        <div class="bg-img">
            <div class="container top-footer d-flex justify-content-between">
                <div v-for="(link, index) in actionLinks" :key='index'>
                    <h4>{{ link.title }}</h4>
                    <ul>
                        <li v-for="(subLink, subIndex) in link.links" :key="subIndex">{{ subLink }}</li>
                    </ul> 
                </div> 
                <div>
                    <img src="/img/dc-logo-bg.png" alt=""> 
                </div>
            </div>
            
        </div>
        <div class=" container bottom-footer d-flex justify-content-between align-items-center">

                <button type="button" class="btn btn-secondary btn-lg">SIGN UP</button>

            <div class="d-flex justify-content-between align-items-center ">
                <span><strong>FOLLOW US</strong></span>
                <img v-for="img in mediaLogos" :src="img.social" alt="">
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
                            'Characters',
                            'Comics',
                            'Movies',
                            'TV',
                            'Games',
                            'Videos',
                            'News' 
                        ]
                    },
                    {
                        title:  'SHOP',
                        links: [
                            'Shop DC',
                            'Shop DC Collectibles'
                        ]
                    },
                    {
                        title:  'DC',
                        links: [
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
                        ]
                    },
                    {
                        title:  'SITES',
                        links: [
                            'DC',
                            'MAD Magazine',
                            'DC Kids',
                            'DC Universe',
                            'DC Power Visa' 
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
    height: 300px;
    background-image: url('/img/footer-bg.jpg');
  }
  h4{
    font-size: 0.9rem;
    color: white;
  }
  li{
    color: lightgray;
    font-size: 0.7rem;
  }
  ul{
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .top-footer img{
    display: block;
    width: 300px;
  }
</style>