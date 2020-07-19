<template>
    <section>
        <div class="services container">
            <h2>Առաջարկվող ծառայություների փաթեթ</h2>
            <div class="grid">
                <div v-for="item in items" :key="item.id" class="grid-item">
                    <img :src="item.img" :alt="item.title">
                    <h4>{{ item.title }}</h4>
                    <p>{{ item.description }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import marketing from '../assets/marketing.png'
    import cragravorum from '../assets/cragravorum.png'
    import dizayn from '../assets/dizayn.png'
    import seo from '../assets/seo.png'
    import smm from '../assets/smm.png'
    import brand from '../assets/brand.png'

    export default {
        name: 'Services',
        data() {
            return {
                items: [
                    {
                        id: 1,
                        img: marketing,
                        title: 'Մարքեթինգ',
                        description: 'Մարքեթինգը յուրօրինակ միջոց է առաջարկելու սպառողներին օպտիմալ գներ, զարգացնել և առաջխաղացնել ապրանքը շուկայում:'
                    },
                    {
                        id: 2,
                        img: cragravorum,
                        title: 'Ծրագրավորում',
                        description: 'Պատրաստում ենք որակյալ կայքեր: Կայքի պատրաստման մեջ ներառվում է խորհրդատվությունը, դիզայնը և ծրագրավորումը:'
                    },
                    {
                        id: 3,
                        img: dizayn,
                        title: 'Վեբ դիզայն',
                        description: 'Վեբ կայքերի, մոբայլ հավելվածների նախագծում (UX) և UI դիզայն ժամանակակից լուծումներով և ստանդարտներով։'
                    },
                    {
                        id: 4,
                        img: seo,
                        title: 'SEO օպտիմիզացում',
                        description: 'Կայքերի առաջխաղացում, կայքի դիրքերի բարելավում որոնողական համակարգերում (Google, Yandex)'
                    },
                    {
                        id: 5,
                        img: smm,
                        title: 'SMM',
                        description: 'SMM-ը մի հարթակ է, որ օգնում է ձեռք բերել նկատելի ազդեցություն և ապրանքանիշի տեսանելիություն։ SMM-ը բիզնեսի առաջմղման արդյունավետ գործիք է:'
                    },
                    {
                        id: 6,
                        img: brand,
                        title: 'Բրենդինգ',
                        description: 'Լոգոներ, վիզիտկաներ, բուկլետներ, վեկտորային նկարներ, պիտակներ, գովազդներ (նաև ինտերնետային), բրենդինգ և այլ ծառայություններ, որոնք կապված են գրաֆիկ դիզայնի հետ։'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    section { background-color: rgb(255, 255, 255);}
    .container {
        max-width: 1140px;
        margin: 0 auto;
    }
    .services {
        padding: 20px 20px 40px 20px;
        text-align: center;
    }
    h2 {
        margin: 20px 0 50px 0;
        color:rgb(102, 102, 102)    
    }
    h4 {
        margin: 0;
        font-weight: 600;
        font-size: 18px;
        color: rgb(68, 68, 68);
        font-family: 'Roboto', sans-serif;
    }
    p {
        color: rgb(102, 102, 102);
        font-family: 'Roboto', sans-serif;
        font-weight: 100;
    }
    .grid {
        display: grid;
        grid-template-columns: auto auto auto;
    }
    .grid-item img {
        margin: 10px auto;
        width: 120px;
        height: 120px;
    }
    .grid-item {padding: 10px;}
    @media screen and (max-width: 960px) {
        .grid {
            grid-template-columns: auto auto;
        }
    }
    @media screen and (max-width: 576px) {
        .grid {
            grid-template-columns: auto;
        }
    }
</style>