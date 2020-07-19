<template>
    <div class="menu" :style="[num ? dis : nodis]" @click="hideBar(0)">
        <div class="bar" :style="[num ? show : hide]">
            <h3>Danisoft</h3>
            <ul>
                <li><a href="#">Our works</a></li>
                <li><a href="#">Lessons</a></li>
                <li><a href="#">News</a></li>
                <li><a href="#">About us</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Menu',
        props: {
            num: { type: Number, required: true }
        },
        data() {
            return {
                show: { transform: 'translate(0, 0)' },
                hide: { transform: 'translate(300px, 0)' },
                dis: { display: '', 'z-index': 1 },
                nodis: { opacity: 0, width: 0 }
            }
        },
        methods: {
            hideBar(item) {
                this.$emit('updateNum', item)
            }
        }
    }
</script>

<style scoped>
    .menu {
        position: fixed;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.65);
        overflow: hidden;
        bottom: 0;
        font-family: 'Roboto', sans-serif;
    }
    .bar {
        text-align: center;
        width: inherit;
        height: inherit;
        width: 300px;
        padding-top: 18px;
        font-size: 18px;
        background-color: rgb(241, 241, 241);
        color: rgb(68, 68, 68);
        float: right;
        transition-duration: 0.5s;
    }
    h3 {
        margin: 0 0 18px 0;
        font-weight: 600;
    }
    ul {
        list-style: none;
        margin: 0;
        padding: 0;
        width: 100%;
    }
    li {
        padding: 8px 0;
        cursor: pointer;
    }
    a {
        width: inherit;
        padding: 8px 16px;
        text-decoration: none;
        color:rgb(68, 68, 68)
    }
    li:hover {
        background-color: #e2e3e4
    }
</style>