<script>
export default{
    name: 'CardMainComp',
    props: {
        img: String,
        textContent: String,
    }
}
</script>

<template>
    <div class="my-card">
        <img :src="img" alt="">
        <h5>
            {{ textContent }}
        </h5>
    </div>
</template>

<style lang="scss" scoped>
    .my-card{
        flex-basis: calc(100%/6 - 15px);
        display: flex;
        flex-direction: column;
        img{
            width: 100%;
            aspect-ratio: 1;
            display: block;
        }

        h5{
            margin-top: 5px;
            font-size: 12px;
        }
    }
</style>