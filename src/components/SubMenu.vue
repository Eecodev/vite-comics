<template>
    <div>
        <ul>
            <li v-for="(link, index) in links" :key="index">{{ link }}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'SubMenu',
        props:[
            'links',
        ]
    }
</script>

<style lang="scss" scoped>

</style>