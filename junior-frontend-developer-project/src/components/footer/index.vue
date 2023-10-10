<template>
    <footer class="contener">
        <div class="borier">
            <div class="borier1"></div>
            <div class="borier2"></div>
        </div>
        <div class="footer">
            <div class="center">
                <div class="left">
                    <router-link class="link" to="">Календарь мероприятий</router-link>
                    <router-link class="link" to="">Провести мероприятие</router-link>
                    <router-link class="link" to="">Стать арендатором</router-link>
                    <router-link class="link" to="">Наши проекты</router-link>
                    <router-link class="" to="">Контакты</router-link>
                </div>
                <div class="right">
                    <p>Подпишись и будь в курсе происходящего</p>
                    <div class="form">
                        <div class="input_button">
                            <input type="text">
                            <button>Подписаться</button>
                        </div>
                        <div class="checkbox">
                            <div class="mark"></div>
                            <p>Соглащение на обработку данных</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="under">
                <div class="politik">
                    <div class="side">
                        <p>© Millennials 2022</p>
                        <a href="">Политика конфидициальности</a>
                    </div>
                    <p>Cookis</p>
                </div>
                <img src="/Image/соц. сети.svg" alt="">
                <div class="tagree">
                    <p>Создание и продвижение</p>
                    <img class="img_tagree" src="/Image/tagree.svg" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>


<script>
export default{
    name:"FooterBlock"
}
</script>


<style lang="scss">
footer{
    .borier{
        display: flex;
        justify-content: space-around;
        .borier1{
            width: 42.8%;
            height: 2px;
            flex-shrink: 0;
            background: var(--1-liner, linear-gradient(270deg, #1C1B1B 0%, rgba(255, 255, 255, 0.00) 82.86%));
        }
        .borier2{
            width: 42.8%;
            height: 2px;
            flex-shrink: 0;
            background: linear-gradient(90deg, #1C1B1B 0%, rgba(255, 255, 255, 0.00) 100%);
        }
    }
    .footer{
        .center{
            margin-top: 60px;
            display: flex;
            justify-content: space-between;
            .left{
                border-left: 4px solid #BC3324;
                padding-left: 22px;
                display: flex;
                flex-direction: column;
                .link{
                    margin-bottom: 22px;
                }
            }
            .right{
                .form{
                    .input_button{
                        margin: 24px 0 15px;
                    }
                }
            }
        }
        .under{
            display: flex;
            justify-content: space-between;
            margin-top: 100px;
            .politik{
                width: 384px;
                max-width: 100%;
                display: flex;
                align-items: flex-end;
                justify-content: space-between;
                .side{
                    p{
                        margin-bottom: 20px;
                    }
                }
            }
            .tagree{
                display: flex;
                align-items: flex-end;
                .img_tagree{
                    margin-left: 15px;
                }
            }
        }
    }
    
}

</style>