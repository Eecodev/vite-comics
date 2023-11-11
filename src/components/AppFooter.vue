<template>
    <footer>
        <div class="bg-img">
            <div class="container top-footer d-flex justify-content-around">
                <div v-for="(link, index) in actionLinks" :key='index' class="">
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
import { actionLinks } from '../data/data.js';
import { mediaLogos } from '../data/data.js';
    export default {
        name: 'AppFooter',
        data(){
            return{
                action: actionLinks,
                logos: mediaLogos
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