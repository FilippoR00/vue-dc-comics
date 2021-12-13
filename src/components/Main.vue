<template>
    <div class="main">
        <div class="container">
            --> Content goes here &#60;--
        </div>
    </div>
</template>

<script>
    export default {
        name : 'myMain',
    }
</script>

<style scoped lang="scss">
    @import '../assets/style/global.scss';
    .main{
        background-color: #000;
        color: white;

        // temp *************************
        height: 130px;
        display: flex;
        font-size: 25px;
        font-weight: 600;
    }
</style>