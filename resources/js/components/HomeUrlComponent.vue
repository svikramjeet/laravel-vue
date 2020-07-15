<template>
    <div class="links" v-if="links">
        <a v-for="(item, index) in links" :href="item">{{index}}</a>
    </div>
</template>

<script>
    export default {
        props: ['links'],
        mounted() {
            console.log('Component HomeUrl mounted with props')
        }
    }
</script>
