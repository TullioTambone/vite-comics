<script>
    export default{
        name: 'Header',

        data() {
            return{
                cta: 0,
                links: [
                    {
                        url: '/',
                        name: 'CHARACTERS',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'COMICS',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'MOVIES',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'TV',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'GAMES',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'COLLECTIBLES',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'VIDEOS',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'FANS',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'NEWS',
                        control: false,
                    },
                    {
                        url: '/',
                        name: 'SHOP',
                        control: false,
                    },
                ]
            }
        },
        methods: {
            changeIndex(i){
                this.cta  = i
            }
        }
    }
</script>

<template>
    <header>
        <nav>
            <img src="/vue-dc-comics-1/img/dc-logo.png" alt="">
            <div>
                <ul>
                    <li v-for="(element, index) in links" :key="index" :class="(cta == index) ? 'active' : ''" @click="changeIndex(index)">
                        <a>{{ element.name }}</a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style lang="scss">
</style>