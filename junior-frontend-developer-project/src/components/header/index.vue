<template>
    <header class="contener">
        <img src="/Image/logo (1).svg" alt="logo">
        <div class="link">
            <router-link to="">Мероприятия</router-link>
            <router-link class="two" to="">Блог</router-link>
            <router-link class="frea" to="">О Нас</router-link>
            <router-link to="">Контакты</router-link>
        </div>
        <button class="text-button">Войти</button>
    </header>
</template>

<script>
export default{
    name:"HeaderBlock",
}
</script>

<style lang="scss">
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #DEDEDE80 50%;
    backdrop-filter: blur(10px);
    img{
        width: 202px;
        height: 147px; 
    }
    .link{
        .two{
            margin: 50px;
        }
        .frea{
            margin-right: 50px;
        }
    }
}

</style>