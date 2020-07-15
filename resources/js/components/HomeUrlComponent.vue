<template>
    <div class="links" v-if="links">
        <a v-for="(item, index) in links" :href="item">{{index}}</a>
    </div>
</template>

<script>
    export default {
    data() {
        return {
            links: { 
                Docs: "https://laracasts.com/docs",
                News: "https://laravel-news.com",
                Laracasts: "https://laracasts.com",
                Nova: "https://nova.laravel.com",
                Forge: "https://forge.laravel.com",
                Vapor: "https://vapor.laravel.com",
                GitHub: "https://github.com/laravel/laravel"
                },
        }
    },
    mounted() {
        console.log('Component HomeUrl mounted.')
    }
    }
</script>
