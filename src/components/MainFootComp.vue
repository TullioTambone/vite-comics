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
    <div id="footer-main">
        <div class="container">
            <ul>
                <li v-for="(element, index) in images" :key="index">
                    <img :src="element.url" alt="">
                    {{ element.title }}
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#footer-main{
    background-color: rgb(12,124,236);
    color: white;
    width: 100%;
    padding: 2em 5rem;
    position: relative;
    z-index: 99;
    ul{
        display: flex;
        justify-content: space-between;
        li{
            list-style-type: none;
            display: flex;
            align-items: center;
            font-size: 10px;
            
            img{
                width: 50px;
                display: block;
                margin-right: 1em;
            }
        }
    }
}
</style>