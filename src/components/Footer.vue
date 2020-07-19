<template>
    <footer>
        <div class="footer">
            <div class="flex">
                <img src="../assets/logo.png" alt="logo">
                <div class="flex-right">
                    <div class="soc-media">
                        <a href="#">
                            <i class="fa fa-facebook-square" aria-hidden="true"></i>
                        </a>
                        <a href="#">
                            <i class="fa fa-instagram" aria-hidden="true"></i>
                        </a>
                        <a href="#">
                            <i class="fa fa-telegram" aria-hidden="true"></i>
                        </a>
                    </div>
                    <div class="share">
                        <a href="#" class="btn">
                            <span>

                            </span>
                            Հավանել
                        </a>
                        <a href="#" class="btn">Կիսվել</a>
                    </div>
                </div>
                
            </div>
            <div class="copy-right">
                copyRight &#169; <strong>Danisoft</strong>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'Footer',
        
    }
</script>

<style scoped>
    footer {
        padding: 20px;
        background-color: rgb(35, 43, 54);
    }
    .footer {
        max-width: 1872px;
        padding:  0 24px;
        margin: 0 auto
    }
    img {
        width: 70px;
        height: 70px;
    }
    .copy-right {
        text-align:  center;
        font-family: 'Roboto', sans-serif;
        color: rgb(255, 255, 255)
    }
    .flex {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .flex-right { display: flex }
    .soc-media { padding: 20px 24px }
    .share {
        padding: 20px 0;
        font-family: 'Roboto', sans-serif;
    }
    .soc-media a {
        color:rgb(255, 255, 255);
        margin: 0 10px
    }
    .btn {
        color: rgb(255, 255, 255);
        background-color: rgb(66, 103, 178);
        border: 1px solid rgb(66, 103, 178);
        text-decoration: none;
        padding: 2px 4px;
        margin: 0 2px;
        font-size: 12px;
        border-radius: 4px;
    }
    @media screen and (max-width: 576px) {
        .soc-media {
            display: flex;
            flex-direction: column;
        }
        .soc-media a { margin: 1px 0 }
        .footer { padding: 0 12px }
    }
</style>