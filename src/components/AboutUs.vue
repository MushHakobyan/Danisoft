<template>
    <section>
        <h1>Մեր Մասին</h1>
        <div class="about">
            <div class="about-us">
                <h3>Մենք տաղանդ ունենք տեխնոլոգիայի ապագան փոխակերպելու:</h3>
                <p>Մենք զբաղվում ենք վեբ կայքերի մշակմամբ նրանց՝ հետագա աջակցությամբ և առաջխաղացմամբ: Մենք հանդես ենք գալիս որպես օղակ հաճախորդի և նրա նոր հաճախորդների միջև՝ հնարավորինս արտացոլելով ընկերության ուշադրությունը կայքերի և դրա նպատակների վրա: Այնուամենայնիվ մենք փնտրում ենք յուրահատուկ մոտեցում յուրաքանչյուր հաճախորդի նկատմամբ՝ փորձելով ստեղծել իրենց կայքը:</p>
            </div>
            <div>
                <img src="../assets/home_about.png" alt="home">
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'AboutUs'
    }
</script>

<style scoped>
    h3, p {
            font-family: 'Roboto', sans-serif;
    }
    section {
        text-align: center;
        padding: 20px;
        color: rgb(255, 255, 255);
    }
    h1 { 
        margin: 0 0 50px 0;
        font-size: 32px;
    }
    .about {
        padding: 62px 32px;
        display: flex;
        justify-content: center;
    }
    .about-us {
        padding: 30px 20px;
        width: 448px;
        height: 610px;
        box-sizing: border-box;
        overflow: hidden;
    }
    p {
        text-align: justify;
        font-weight: 100;
    }
    img {
        margin: 0 47px;
        width: 354px;
        height: 400px;
    }
    @media screen and (max-width: 960px) {
        .about {
            flex-direction: column;
            align-items: center;
        }
        .about-us {
            width: 90%;
            height: auto;
        }
        img {
            width: 90%;
            height: auto;
        }
    }
</style>