<template>
    <div class="navbar">
        <div class="container">
            <div class="logo">
                <img src="../assets\img\dc-logo.png" alt="">
            </div>
            <div class="nav-menu">
                <ul>
                    <li v-for="(item, index) in items" :key="index" :class="{ active : item.status}"><a :href="item.url">{{item.text}}</a></li>
                </ul>
            </div>
        </div>
    </div>




</template>

<script>
    export default {
        name : 'header',
        data() {
            return {
                items: [
                    {
                        text: "characters",
                        url: "#",
                        status: false
                    },
                    {
                        text: "comics",
                        url: "#",
                        status: true
                    },
                    {
                        text: "movies",
                        url: "#",
                        status: false
                    },
                    {
                        text: "tv",
                        url: "#",
                        status: false
                    },
                    {
                        text: "games",
                        url: "#",
                        status: false
                    },
                    {
                        text: "collectibles",
                        url: "#",
                        status: false
                    },
                    {
                        text: "videos",
                        url: "#",
                        status: false
                    },
                    {
                        text: "fans",
                        url: "#",
                        status: false
                    },
                    {
                        text: "news",
                        url: "#",
                        status: false
                    },
                    {
                        text: "shop",
                        url: "#",
                        status: false
                    },
                ]
            }
        },
    }
</script>

<style scoped lang="scss">
    @import '../assets/style/global.scss';
    .navbar{
        .container{
            height: 120px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo{
            img{
                width: 80px;
            }
        }
        .nav-menu{
            ul{
                list-style: none;
                display: flex;
                >:hover{
                        border-bottom: 5px solid $mainColor;
                    }
                li{
                    margin: 0px 10px;
                    line-height: 115px;
                    transition: 0.3s;
                    transition-timing-function: ease-in-out;
                    a{
                        color: #303030;
                        text-decoration: none;
                        text-transform: uppercase;
                        font-size: 14px;
                        font-weight: 600;
                        padding: 5px;
                        font-family: 'Roboto Condensed', 'Roboto', Arial, Helvetica, sans-serif;
                    }
                    :hover{
                        color: $mainColor;
                    }
                }
            }
        }
    }

    .active{
        border-bottom: 5px solid $mainColor;
    }
</style>