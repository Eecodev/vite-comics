<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center border">
            <div>
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </div>
            <div>
                <ul class="d-flex justify-content-between">
                    <li class="p-3" v-for="navLink in navLinks">
                        <a href="#">{{ navLink }}</a>
                    </li>
                </ul>  
            </div>
        </div>
    </header>
</template>
  
<script>
    export default {
        name: 'AppHeader',
        components: {

        },
        data(){
            return{
                navLinks: [
                    'CHARACTERS',
                    'COMICS',
                    'MOVIES',
                    'TV',
                    'GAMES',
                    'COLLECTIBLES',
                    'VIDEOS',
                    'FANS',
                    'NEWS',
                    'SHOP'
                ],
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
    }
  }
</style>