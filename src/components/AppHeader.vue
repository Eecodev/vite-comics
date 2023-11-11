<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center border">
            <div>
                <img src="/public/img/dc-logo.png" alt="Logo">
            </div>
            <div>
                <ul class="d-flex flex-wrap">
                    <li class="p-3" v-for="navLink in navLinks">
                        <a href="#">{{ navLink }}</a>
                    </li>
                </ul>  
            </div>
        </div>
    </header>
</template>
  
<script>
import { navLinks } from '../data/data.js';
    export default {
        name: 'AppHeader',
        components: {

        },
        data(){
            return{
                links: navLinks
            }
        },
        methods: {

        }
    };
    
</script>
  
<style lang="scss" scoped>
  ul{
    list-style-type: none;
    
    a{
        text-decoration: none;
        color: var(--dark);
    }
  }
</style>