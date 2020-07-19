<template>
    <section>
        <h1>Պարզ գործընթաց՝ գաղափարից մինչև գործարկել</h1>
        <div class="flex">
            <div v-for="item in items" :key="item.id" class="flex-item grid-item">
                <div class="item">
                    <img :src="item.img" alt="media">
                    <a href="#" class="item-btn">
                        <i class="fa fa-paperclip" aria-hidden="true"></i>
                    </a>
                    <div class="tr-left">{{ item.title }}</div>
                    <div class="tr-bottom">{{ item.desc }}</div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import media from '../assets/media.png'
    import html from '../assets/html.png'
    import search from '../assets/search.png'

    export default {
        name: 'SimpleProcess',
        data() {
            return {
                items: [
                    {
                        id: 1,
                        img: media,
                        title: 'ՓՈՐՁ 2',
                        desc: 'Հակառակ ընդհանուր պատկերացմանը...'
                    },
                    {
                        id: 2,
                        img: html,
                        title: 'ՓՈՐՁ 3',
                        desc: 'Հակառակ ընդհանուր պատկերացմանը...'
                    },
                    {
                        id: 3,
                        img: search,
                        title: 'SEO ՕՊՏԻՄԻԶԱՑՈՒՄ',
                        desc: 'Հակառակ ընդհանուր պատկերացմանը...'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    section {
        padding: 20px 20px 40px 20px;
        text-align: center;
    }
    h1 {
        margin: 0 0 50px 0;
        font-size: 32px;
        font-family: "Cookie",cursive;
        color: rgb(68, 68, 68)
    }
    .flex {
        display: flex;
        justify-content: center;
    }
    .flex-item {
        position: relative;
        width: 358px; 
        padding: 16px;
    }
    .item {
        cursor: pointer;
        position: relative;
        overflow: hidden;
        height: inherit;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        font-family: Roboto, sans-serif;
        box-shadow: 0 4px 5px 0 rgba(0,0,0,.24);
    }
    .item img {
        width: 100%;
        height: 100%;
        z-index: -1;
    }
    .tr-left, .tr-bottom {
        position: absolute;
        transition-duration: 0.5s;
    }
    .item:hover { background-color: rgba(0, 0, 0, 0.6) }
    .item-btn {
        position: absolute;
        top: 45%;
        display: none;
        font-size: 18px;
        color: rgb(255, 255, 255);
    }
    .item-btn:hover { color:rgb(255, 68, 68) }
    .item:hover .item-btn { display: inline } 
    .item:hover .tr-bottom { bottom: 10px }
    .item:hover .tr-left { left: 10px }
    .tr-left {
        left: -100%;
        bottom: 30px;
        color: rgb(255, 68, 68);
        font-weight: 500;
    }
    .tr-bottom {
        bottom:  -30px;
        left: 10px;
        color:rgb(255, 255, 255)
    }
    @media screen and (max-width: 960px) {
        .flex {
            flex-direction: column;
            align-items: center;
        }
        .flex-item { width: 95% }
    }
</style>