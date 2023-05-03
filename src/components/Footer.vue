<script>
    export default{
        name: 'Footer',
        
        data() {
            return{
                footerList: [
                    {
                        control: false,
                        title:'DC COMICS',
                        subList: [
                            {
                                subTitle:'Characters'
                            },
                            {
                                subTitle:'Comics'
                            },
                            {
                                subTitle:'Movies'
                            },
                            {
                                subTitle:'TV'
                            },
                            {
                                subTitle:'Games'
                            },
                            {
                                subTitle:'Videos'
                            },
                            {
                                subTitle:'News'
                            },

                        ]
                    },
                    {
                        control: true,
                        title:'SHOP',
                        subList: [
                            {
                                subTitle: 'Shop DC'
                            },
                            {
                                subTitle: 'Shop DC Collectibles'
                            }
                        ]
                    },
                    {
                        control: false,
                        title:'DC',
                        subList: [
                            {
                                subTitle:'Term Of Use'
                            },
                            {
                                subTitle:'Privacy policy(New)'
                            },
                            {
                                subTitle:'Ad Choices'
                            },
                            {
                                subTitle:'Advertising'
                            },
                            {
                                subTitle:'jobs'
                            },
                            {
                                subTitle:'Subscriptions'
                            },
                            {
                                subTitle:'Talent Workshops'
                            },
                            {
                                subTitle:'CPSC Certificates'
                            },
                            {
                                subTitle:'Ratings'
                            },
                            {
                                subTitle:'ShopHelp'
                            },
                            {
                                subTitle:'Contact Us'
                            },
                        ]
                    },
                    {
                        control: false,
                        title:'SITIES',
                        subList:[
                            {
                                subTitle:'DC'
                            },
                            {
                                subTitle:'MAP Magazine'
                            },
                            {
                                subTitle:'DC Kids'
                            },
                            {
                                subTitle:'DC Universe'
                            },
                            {
                                subTitle:'DC Power Visa'
                            },

                        ]
                    }
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <div id="up-footer">
            <div class="container">
                <div id="footer-list">
                    <ul v-for="(element, index) in footerList" :key="index" 
                    :class="(element.control == true) ? 'my-position' : ''">
                        <h3>{{ element.title }}</h3>
                        <li v-for="(elem, i) in element.subList" :key="i">
                            {{ elem.subTitle }}
                        </li>
                    </ul>
                </div>
                <img src="/vue-dc-comics-1/img/dc-logo-bg.png" alt="">
            </div>
        </div>
        <div id="down-footer">
            <div class="container">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div>
                    <span>
                        FOLLOW US
                    </span>
                </div>
            </div>
        </div>
    </footer>
</template>

<style>
</style>