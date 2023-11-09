<template>
    <main>
        <div class="top-main">
            <div class="container py-5">
                <h2>content goes here</h2>
            </div>
        </div>
        <div class="bottom-main">
            <div class="container py-5">
               <ul class="d-flex justify-content-between">
                    <li v-for="el in mainImgs" :key="index">
                        <a href="">
                            <img :src="el.img" alt="" class="px-2 w-25 h-75">
                            {{el.text}}
                        </a>
                    </li>
               </ul>
            </div>
        </div>

    </main>
</template>
  
<script>
    export default {
        name: 'AppMain',
        data(){
            return{
                mainImgs:[
                    {
                        img: "/src/assets/img/buy-comics-digital-comics.png",
                        text: 'DIGITAL COMICS'
                    },
                    {
                        img: "/src/assets/img/buy-comics-merchandise.png",
                        text: 'DC MERCHANDISE'
                    },
                    {
                        img: "/src/assets/img/buy-comics-shop-locator.png",
                        text: 'SUBSCRIPTION'
                    },
                    {
                        img: "/src/assets/img/buy-comics-subscriptions.png",
                        text: 'COMIC SHOP LOCATOR'
                    },
                    {
                        img: "/src/assets/img/buy-dc-power-visa.svg",
                        text: 'DC POWER VISA'
                    },
                    
                ]
            }
        }
    };
    
</script>
  
<style lang="scss" scoped>
    .top-main{
        background-color: #1c1c1c;
    }
    .bottom-main{
        background-color: #0282f9;
    }
</style>