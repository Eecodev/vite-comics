<template>
    <footer>
        <div class="bg-img">
            <div class="container top-footer">
                
            </div> 
        </div>
        <div>
            <div class="container bottom-footer">
                <button type="button" class="btn btn-secondary btn-lg">SIGN UP</button>
            </div> 
        </div>
    </footer>
</template>
  
<script>
    export default {
        name: 'AppFooter',
        data(){
            return{
                actionlinks:[
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
                ]
            }
        }
       
    };
    
</script>
  
<style lang="scss" scoped>
  .bg-img{
    height: 450px;
    background-image: url('/public/img/footer-bg.jpg');
  }
</style>