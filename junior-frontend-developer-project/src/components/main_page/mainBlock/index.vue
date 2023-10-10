<template>
    <div class="mainBlock">
        <h2 >АРТ-ПРОСТРАНСТВО</h2>
        <img src="/Image/LENNI.svg" alt="">
        <h2>ДЛЯ ЛЮДЕЙ, ГОРЯЩИХ СЕРДЦЕМ И ДЕЛОМ МЕСТО ДЛЯ НАСТОЯЩЕГО</h2>
        <p>Я хочу</p>
        <div class="button">
            <button class="text-button read">Провести мероприятие</button>
            <button class="text-button ">Стать арендатором</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainBlock"
}
</script>

<style lang="scss">
.mainBlock {
    display: flex;
    flex-direction: column;
    align-items: center;
    img {
        width: 100%;
        margin: 70px 0;
        
    }
    p{
        margin: 100px 0 46px;
    }
    .button{
        width: 34%;
        display: flex;
        justify-content: space-between;
        .read{
            border: none;
            background-color: #BC3324;
            color: white;
        }
    }
}
</style>