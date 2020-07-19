<template>
    <section>
        <div class="header-sec">
            <span>ԽԵՆԹ ԳԱՂԱՓԱՐՆԵՐ: ԱՅՍՊԵՍ ԵՆՔ ԿԱՌՈՒՑՈՒՄ ՎԱՂՎԱ ԱՇԽԱՐՀԸ ԱՅՍՕՐ</span>         
            <img src="../assets/home1.png" alt="home1">
        </div>
    </section>
</template>

<script>
    export default {
        name: 'HeaderSec'
    }
</script>

<style scoped>
    section {
        height: 400px;
        background-image: url('../assets/home.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        display: flex;
        align-items: flex-end;
        justify-content: center;
    }
    img {
        width: 500px;
        width: 300px;
    }
    .header-sec {
        display: flex;
        justify-content: center;
        align-items: center;
        height: auto;
        overflow: hidden;
    }
    span {
        color: rgb(255, 68, 68);
        font-size: 18px;
        font-weight: 700;
        margin-bottom: 80px;
        text-shadow: -1px -1px 1px #000;
        text-align: center;
    }
    @media screen and (max-width: 768px) {
        .header-sec {
            flex-direction: column;
            align-items: center;
            /* padding-top: 560px; */
        }
        span {
            margin: 0;
            text-align: center;
        }
        img {
            width: 100%;
            height: auto;
        }
        section {
            padding-top: 160px;
        }
    }
    @media screen and (max-width: 576px) {
        section {
            padding-top: 0;
        }
    }
</style>