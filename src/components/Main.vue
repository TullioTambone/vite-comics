<script>
    export default{
        name: 'Main',
        
        data() {
            return{
                images: [
                    {
                        title: 'DIGITAL COMICS',
                        url: '/vue-dc-comics-1/img/buy-comics-digital-comics.png'
                    },
                    {
                        title: 'DC MERCHANDISE',
                        url: '/vue-dc-comics-1/img/buy-comics-merchandise.png'
                    },
                    {
                        title: 'SUBSCRIPTION',
                        url: '/vue-dc-comics-1/img/buy-comics-subscriptions.png'
                    },
                    {
                        title: 'SUBSCRIPTION',
                        url: '/vue-dc-comics-1/img/buy-comics-shop-locator.png'
                    },
                    {
                        title: 'COMIC SHOP LOCATIOR',
                        url: '/vue-dc-comics-1/img/buy-dc-power-visa.svg'
                    }
                ]
            }
        }
    }
</script>

<template>
    <main>
        <div  class="container">Contenuto post</div>
        <div id="footer-main">
            <ul>
                <li v-for="(element, index) in images" :key="index">
                    <img :src="element.url" alt="">
                    {{ element.title }}
                </li>
            </ul>
        </div>
    </main>
</template>

<style lang="scss">

</style>