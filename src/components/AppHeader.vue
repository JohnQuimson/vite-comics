<script>
export default{
    name: 'Header',
    data(){
        return {
            navbarElements: [
                {
                    nome: 'characters',
                    link: '#',
                },
                {
                    nome: 'comics',
                    link: '#',
                },
                {
                    nome: 'movies',
                    link: '#',
                },
                {
                    nome: 'tv',
                    link: '#',
                },
                {
                    nome: 'games',
                    link: '#',
                },
                {
                    nome: 'collectibles',
                    link: '#',
                },
                {
                    nome: 'videos',
                    link: '#',
                },
                {
                    nome: 'fans',
                    link: '#',
                },
                {
                    nome: 'news',
                    link: '#',
                },
                {
                    nome: 'shop',
                    link: '#',
                },
            ],
        };
    },
};
</script>

<template>
    <header>
        <div class="logo">
            <div class="cont-logo">
                <img src="../../public/img/dc-logo.png" alt="">
            </div>  
        </div>
        <ul class="navbar">
            <li v-for="li in navbarElements">
                <span>{{ li.nome }}</span>
            </li>
        </ul>
    </header> 
</template>

<style scoped lang="scss">
@use '../styles/general' as *;

</style>