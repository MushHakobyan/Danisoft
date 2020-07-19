<template>
    <header>
        <div class="header">
            <div class="header-logo">
                <img src="../assets/logo.png" alt="logo.png" height="80px" width="80px">
            </div>
            <div class="header-icons">
                <ul class="icon-list">
                    <li class="home">
                        <a href="#">
                            <i class="fa fa-home" aria-hidden="true"></i>
                        </a> 
                    </li>
                    <li class="lang">
                        <span>
                            <img src="../assets/arm.png" alt="arm-flag" width="18px" height="auto">
                        </span>
                    </li>
                    <li class="bar" @click="showBar">
                        <i class="fa fa-bars" aria-hidden="true"></i>
                    </li>
                </ul>            
            </div>
        </div>
        <Menu :num="num" @updateNum='updateNumber' /> 
    </header>
</template>

<script>
    import Menu from './Menu'

    export default {
        name: 'Header',
        components: { Menu },
        data() {
            return {
                num: 0
            }
        },
        updated() {
            if(this.num == 1) {
                document.body.style.overflow = 'hidden'
            } else {
                document.body.style.overflow = ''   
            }
        },
        methods: {
            showBar() {
                this.num = 1
            },
            updateNumber(item) {
                this.num = item
            }
        }
    }
</script>

<style scoped>
    header {
        position: fixed;
        top: 0;
        width: 100%;
        z-index: 1;
    }
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: rgba(51, 51, 51, 0.8);
        box-shadow: 0 4px 5px 0 rgba(0, 0, 0, 0.24);
    }
    .header-logo, .header-icons { margin: 0 20px }
    .icon-list {
        display: flex;
        list-style: none;
        padding: 0;
    }
    .icon-list > li {
        padding: 0 5px;
        margin: 0 10px;
        cursor: pointer;
    }
    .home i { color: rgb(255, 68, 68) }
    i { font-size: 18px }
    .lang span { padding: 8px }
    .bar i:hover { color: rgb(255, 68, 68) }
    @media screen and (max-width: 576px) {
        header { position: sticky }
    }
</style>