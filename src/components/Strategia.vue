<template>
    <section>
        <div class="sec">
            <h1>Ահա մեր մոտեցումը ձեր նախագիծը</h1>
            <div>
                <div class="flex">
                    <div class="flex-item">
                        <span class="is-num">1</span>
                        <span class="is-title">Ստրատեգիա</span>
                    </div>
                    <div class="flex-item">
                        <img src="../assets/grid1.jpg" alt="grid1" class="flex-img">
                        <img src="../assets/arrow1.png" alt="arrow" class="right-arrow">
                    </div>
                    <div class="flex-item is-text">
    Մենք սահմանում ենք ձեր մրցակցությունը և թիրախային լսարանը: Բացահայտեք, թե ինչ է աշխատում ձեր առցանց արդյունաբերության մեջ, ապա համապատասխանաբար նախագծեք ձեր կայքը:
                    </div>
                </div>
                
                <div class="flex revers">
                    <div class="flex-item is-text">
                        Գույնի սխեման, դասավորությունը, քարտեզը և ոճը: Մենք ձեր ապրանքանիշը կյանքի ենք կոչելու մի յուրօրինակ գլուխգործոցով, որը կառուցված է հենց ձեզ համար
                    </div>
                    <div class="flex-item">
                        <img src="../assets/arrow2.png" alt="arrow" class="left-arrow">
                        <img src="../assets/grid2.jpg" alt="grid1" class="flex-img">
                    </div>
                    <div class="flex-item">
                        <span class="is-num">2</span>
                        <span class="is-title">Դիզայն</span>
                    </div>
                </div>
               
               <div class="flex">
                    <div class="flex-item">
                        <span class="is-num">3</span>
                        <span class="is-title">Մշակել</span>
                    </div>
                    <div class="flex-item">
                        <img src="../assets/grid3.jpg" alt="grid1" class="flex-img">
                        <img src="../assets/arrow1.png" alt="arrow" class="right-arrow">
                    </div>
                    <div class="flex-item is-text">
    Մենք ձեր գաղափարները վերածում ենք իրականության: & մեր կայքը տեղադրված է «զարգացման սերվերի» վրա, որտեղ դուք ստանում եք դիտելու ամբողջ գործընթացը, ապրեք:
                    </div>
               </div>
               <div class="flex revers">
                    <div class="flex-item is-text">
                        նա այն է, որտեղ դուք ապրում եք կենդանի, աշխարհը: Նախագծում, շուկայավարում և սպասարկում; մենք ձեր կողքին կլինենք ձեր կայքի կյանքի համար:
                    </div>
                    <div class="flex-item">
                        <img src="../assets/arrow2.png" alt="arrow" class="left-arrow">
                        <img src="../assets/grid4.jpg" alt="grid1" class="flex-img">
                    </div>
                    <div class="flex-item">
                        <span class="is-num">4</span>
                        <span class="is-title">Աջակցություն</span>
                    </div>
                </div>    
            </div>
            <div class="btn-content">
               <button class="btn-primary">Get Started</button> 
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Strategia',
    }
</script>

<style scoped>
    .flex {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        font-family: 'Roboto', sans-serif;
    }
    .sec {
        background-image: url('../assets/texture.jpg');
        background-position: center;
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-size: cover;
        position: relative;
        padding: 100px 0 200px;
        clip-path: polygon(0 5%,100% 0,100% 95%,0 100%);
        /* z-index: -1; */
    }
    h1 {
        font-size: 32px;
        color: rgb(255, 255, 255);
        text-align: center;
        margin: 50px 0;
    }
    .flex-item {
        width: 30%;
        padding: 8px;
        display: flex;
        align-items: center;
        height: 405px;
        position: relative;
        justify-content: center;
    }
    .flex-img {
        width: 270px;
        height: 270px;
        border: 10px solid rgba(255, 255, 255, 0.1);
        border-radius: 50%;
        margin: 0 auto;
    }
    .left-arrow, .right-arrow {
        position: absolute;
        bottom: -70px;
    }
    .left-arrow {
        transform: translate(-100px, 0);
    }
    .right-arrow {
        transform: translate(100px, 0);
    }
    .is-text {
        color: rgb(102, 102, 102);
        font-size: 18px;
    }
    .is-title {
        color:rgb(255, 255, 255);
        font-size: 54px;
        position: absolute;
    }
    .is-num {
        color: rgb(255, 73, 124);
        font-size: 180px;
        position: absolute;
        z-index: -1;
    }
    .btn-content {
        display: flex;
        justify-content: center;
        margin-top: 80px;
    }
    .btn-primary {
        padding: 20px 30px;
        font-size: 18px;
        background-color: rgb(255, 255, 255);
        color: rgb(35, 43, 54);
        border: 1px solid rgba(35, 43, 54, 0.55);
        border-radius: 30px;
        cursor: pointer;
        box-shadow: 0 4px 5px 0 rgba(0,0,0,.24);
        outline: none;
        font-family: Arial, Helvetica, sans-serif;
        transition: 0.3s;
    }
    .btn-primary:hover {
        background-color: rgb(35, 43, 54);
        color:rgb(255, 255, 255);
        border-color: rgb(255, 255, 255);
    }
    @media screen and (max-width: 960px) {
        .sec { clip-path: polygon(0 2%,100% 0,100% 98%,0 100%) }
        .flex { flex-direction: column }
        .left-arrow, .right-arrow { display: none }
        .revers { flex-direction: column-reverse }
        .flex-item {
            width: 90%;
            height: 270px;
        }
    }
    @media screen and (max-width: 576px) {
        .sec { clip-path: polygon(0 1%,100% 0,100% 99%,0 100%) }
    }
</style>
