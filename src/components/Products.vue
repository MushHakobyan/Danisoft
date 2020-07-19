<template>
    <section class="section">
        <h1>Ձեր գաղափարը երբեք այնքան լավ տեսք չի ունեցել</h1>
        <hr class="dashed">
        <h4>DaniSoft- ը պատրաստել է ավելի քան 10 միլիոն մարդ</h4>
        <div class="row">
            <div class="col">
                <img src="../assets/61979.png" alt="1212" class="img">
            </div>
            <div class="col">
                <div class="content content-white">
                    <h2>Danisoft.cf</h2>
                    <h6>Համակարգ</h6>
                    <span class="span">
                        <strong>Lang:</strong>
                        HTML, CSS, Bootstrap, jQuery, PHP, Laravel
                    </span>
                    <hr>
                    <span class="span-desc">
                        Սնդի առաքման կայք որով կարող եք պատվիրել ձեզ հարմար ապրանքը այս կայքի միջոցով
                    </span>
                </div>
                <div class="media">
                    <img src="../assets/50687.jpg" alt="" class="media-left">
                    <span class="media-content">"Սա ծատ լավ ձեռնարկ էր մեզ բոլորիս համար"</span>
                </div>
            </div>
        </div>

        <div class="row revers">
            <div class="col">
                <div class="content content-grey">
                    <h2>profcontact.org</h2>
                    <h6>Շինարարական</h6>
                    <span class="span">
                        <strong>Lang:</strong>
                        HTML, CSS, Bootstrap, jQuery, PHP, Laravel
                    </span>
                    <hr>
                    <span class="span-desc">
                        Պրոֆեսիոնալ խոհանոցի տեխնիկայի առաքման կայք որով կարող եք պատվիրել ձեզ հարմար ապրանքատեսակը այս կայքի միջոցով
                    </span>
                </div>
                <div class="media">
                    <img src="../assets/61354.png" alt="" class="media-left is-grey">
                    <span class="media-content">"Ես շատ շնորհակալ եմ ձրի սարքելու համար"</span>
                </div>
            </div>
            <div class="col">
                <img src="../assets/65180.png" alt="1212" class="img">
            </div>
        </div>        

        <div class="row">
            <div class="col">
                <img src="../assets/71514.png" alt="1212" class="img">
            </div>
            <div class="col">
                <div class="content content-white">
                    <h2>Danisoft.tk</h2>
                    <h6>Խանութ</h6>
                    <span class="span">
                        <strong>Lang:</strong>
                        HTML, CSS, Bootstrap, jQuery, PHP, Laravel
                    </span>
                    <hr>
                    <span class="span-desc">
                        Սնդի առաքման կայք որով կարող եք պատվիրել ձեզ հարմար ապրանքը այս կայքի միջոցով
                    </span>
                </div>
                <div class="media">
                    <img src="../assets/5886.jpg" alt="" class="media-left">
                    <span class="media-content">"Ես շատ շնորհակալ եմ այս կայքը ստեղծողի անձնակազմից հիանալի էր իրոք շնորհակալ եմ ձեզ իմ համար սարքելու համար"</span>
                </div>
            </div>
        </div>
        <div class="row revers">
            <div class="col">
                <div class="content content-grey">
                    <h2>rbk</h2>
                    <h6>Բանկաին միջնորդ</h6>
                    <span class="span">
                        <strong>Lang:</strong>
                        HTML, CSS, Bootstrap, jQuery, PHP, Laravel
                    </span>
                    <hr>
                    <span class="span-desc">
                        Եթե ձեզ անհրաժեշտ է սպառոկան վարկ առանց բանկ հաճախելու կարող եք լուծել այդ հարցը
                    </span>
                </div>
                <div class="media">
                    <img src="../assets/77889.jpg" alt="" class="media-left is-grey">
                    <span class="media-content">"Ես շատ շնորհակալ եմ այս կայքը ստեղծողի անձնակազմից հիանալի համակարգ ստեղցելւ համառ իրոք շնորհակալ եմ որ ձրի իմ համար սարքիք"</span>
                </div>
            </div>
            <div class="col">
                <img src="../assets/34023.png" alt="1212" class="img">
            </div>
        </div>  
        <div class="btn-content">
            <button class="btn">Դիտել ավելին</button>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Product'
    }
</script>

<style scoped>
    .section { 
        padding: 50px 20px;
        margin: 0 auto;
    }
    h1 {
        margin: 0 0 5px 0;
        text-align: center;
        color: rgb(255, 68, 68);
        font-size: 32px;
    }
    h4 {
        margin: 0 0 50px 0;
        color:rgb(147, 147, 147);
        text-align: center;
        letter-spacing: 4px;
        font-family: 'Roboto', sans-serif;
    }
    .dashed {
        width: 20%;
        border: 0;
        border-top: 0.1px dashed rgb(102, 102, 102);
    }
    .btn-content {
        margin: 30px 0;
        display: flex;
        justify-content: center;
    }
    .btn {
        padding: 10px 15px;
        background-color: rgb(0, 100, 0);
        font-size: 14px;
        color: rgb(255, 255, 255);
        border: 1px solid rgb(204, 204, 204);
        box-shadow: 0 2px 5px 0 rgba(0,0,0,.24);
        border-radius: 5px;
        font-weight: 600;
        cursor: pointer;
        outline: none;
    }
    .btn:hover { background-color: rgba(3, 121, 3, 0.9) }
    .row {
        padding: 20px;
        display: flex;
        justify-content: center;
        margin: 0 auto;
        width: 888px;
        font-family: 'Roboto', sans-serif;
    }
    .revers { background-color: rgb(255, 255, 255) }
    .col .img {
        width: 428px;
        padding: 1px;
        height: 200px;
        border: 1px solid rgb(204, 204, 204);
    }
    .col {
        padding: 8px;
        width: 428px; 
    }
    h2 {
        margin: 0;
        color: rgb(68, 68, 68)
    }
    h6 {
        margin: 10px 0;
        color: rgb(145, 145, 145);
    }
    .content {
        padding: 20px;
        border: 1.5px solid rgb(204, 204, 204)
    }
    .content-white { background-color: rgb(255, 255, 255) }
    .content-grey { background-color: rgb(238, 238, 238) }
    .span {
        font-size: 12px;
        color: rgb(145, 145, 145)
    }
    .span-desc {
        font-size: 14px;
        color: rgb(102, 102, 102)
    }
    .media {
        padding: 30px;
        display: flex;
    }
    .media-content {
        font-size: 12px;
        color: rgb(167, 167, 167)
    }
    .media-left {
        width: 47px;
        height: 47px;
        padding: 5px;
        margin-right: 20px;
        border-radius: 100%;
        border: 1.5px solid rgb(255, 255, 255)
    }
    .is-grey { border: 1.5px solid rgb(204, 204, 204) }
    @media screen and (max-width: 1280px) {
        .row {
            flex-direction: column;
            align-items: center;
            width: 80%;
        }   
        .col .img, .col {
            width: 100%;
            height: auto;
        }
        .revers { flex-direction: column-reverse }
    }
</style>