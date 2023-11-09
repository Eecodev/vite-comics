<template>
    <header>
        <div class="container">
            <div class="row">
                <div class="col-12 d-flex justify-content-between align-items-center ">
                <img src="../assets/img/dc-logo.png" alt="Logo">
                    <ul class="d-flex justify-content-between">
                        <li class="p-3" v-for="navLink in navLinks">{{ navLink }}</li>
                    </ul> 
                </div>
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
                    'characters',
                    'comics',
                    'movies',
                    'tv',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop'
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
  }
</style>