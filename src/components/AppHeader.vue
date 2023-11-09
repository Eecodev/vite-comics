<template>
    <h1>header</h1>
    <nav>
        <ul>
            <li v-for="navLink in navLinks">{{ navLink }}</li>
        </ul>
    </nav>
</template>
  
<script>
    export default {
        name: 'AppHeader',
        components: {

        },
        data(){
            return{

            }
        },
        methods: {

        }
    };
    
</script>
  
<style lang="scss" scoped>
  
</style>