<script>
    import MainFootComp from './MainFootComp.vue'
    export default{
        name: 'Main',
        components: {
            MainFootComp,
        },
        
        data() {
            return{

            }
        }
    }
</script>

<template>
    <main>
        <div  class="container" id="head-main">
            Contenuto post
        </div>
        <MainFootComp/>
    </main>
</template>

<style>
</style>