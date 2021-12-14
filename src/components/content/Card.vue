<template>
    <div class="card">
        <div class="img">
            <img :src="card.thumb" alt="card.type">
        </div>
        <div class="title">{{card.series}}</div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        card : Object,
    }
}
</script>

<style scoped lang="scss">
    .card{
        width: calc(100% / 6 - 30px);
        .img{
            width: 100%;
            aspect-ratio: 1.1;
            overflow: hidden;
        }
        .title{
            padding: 20px 0px;
            text-transform: uppercase;
            font-size: 15px;
        }
    }

</style>