<template>
    <main>
        <div class="top-main">
            <div class="container py-5">
                <h2>content goes here</h2>
            </div>
        </div>
        <div class="bottom-main">
            <div class="container py-5">
               <ul class="d-flex justify-content-between flex-nowrap ">
                    <li v-for="el in mainImgs">
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
import { cards } from '../data/data';
import { mainImgs } from '../data/data';
    export default {
        name: 'AppMain',
        data(){
            return{
                comics: cards,
                icons: mainImgs
            }
        }
    };
    
</script>
  
<style lang="scss" scoped>
    ul{
        list-style: none;
    }
    .top-main{
        background-color: #1c1c1c;
    }
    .bottom-main{
        background-color: #0282f9;
    }
</style>