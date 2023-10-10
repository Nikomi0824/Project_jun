<template>
    <div class="item">
        <div class="item_up">
        </div>
        <img class="item_img" src="/Image/pic (2).svg" alt="">
        <div class="item_right">
            <p>Мы уже успешно организовали и провели более 100 проектов. Посмотрите, как это было классно.</p>
            <div class="item_button_look">
                <p>Смотреть</p>
                <button class="img-button"><img src="/Image/link (2).svg" alt=""></button>
            </div>
        </div>
    </div>
</template>


<script>
export default{
    name:"ItemBlock"

}

</script>


<style lang="scss">
.item{
    display: flex;
    justify-content: space-between;
    position: relative;
    height: 380px;
    
    .item_up{
        background-color: #BC3324;
        width: 84%;
        height: 246px;
       
    }
    .item_img{
        position: absolute;
        left: 4%;
        width: 52%;
        height: 361.609px;

    }
    .item_right{
        width: 64%;
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        align-items: center;
        .item_button_look{
            margin-top: 89px;
            width: 50%;
            display: flex;
            align-items: center;
        }
    }
}
</style>