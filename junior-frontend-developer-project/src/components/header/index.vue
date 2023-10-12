<template>
    <div class="shell_heder">
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
    </div>
</template>

<script>
export default{
    name:"HeaderBlock",
}
</script>

<style lang="scss">
.shell_heder{
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 11;
    background: #DEDEDE80 ;
    backdrop-filter: blur(10px);
}
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
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