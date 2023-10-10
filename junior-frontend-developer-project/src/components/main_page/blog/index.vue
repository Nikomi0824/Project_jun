<template>
    <div class="contener">
        <h2>Блог</h2>
        <div class="items_block" v-for="(item, index) in items" :key="index">
            <div class="item_block">
                <img :src=item.img alt="">
                <div class="slider_text">
                    <p class="slider_text_up">{{ item.subtext }}</p>
                    <router-link  to="">{{ item.h2 }}</router-link>
                    <div class="slider_text_doun">
                        <p>{{ item.p }}</p>
                        <button class="img-button"><img src="/Image/link (2).svg" alt=""></button>   
                    </div>
                    
                </div>
            </div>
            <img v-if="item.img_border" src="/Image/Rectangle 159.svg" alt="">
        </div>
    </div>
</template>

<script>
export default{
    name:"BlogBlock",
    data(){
        return{
            items:[
                {
                    img:'/Image/фотосессия в стена Театра.jpg',
                    subtext:'26.11.2022',
                    h2:"Фотосессия в стенах Театра драмы",
                    p:"Организовывая фотосессию для локального бренда одежды мы смогли воплотить все пожелания заказчика и у нас получилась отличная работа. Смотрите как это было ",
                    img_border:true
                },
                {
                    img: '/Image/фотосессия в стена Театра.jpg',
                    subtext: '26.11.2022',
                    h2: "Фотосессия в стенах Театра драмы",
                    p: "Организовывая фотосессию для локального бренда одежды мы смогли воплотить все пожелания заказчика и у нас получилась отличная работа. Смотрите как это было ",
                    img_border: true
                },
                {
                    img: '/Image/фотосессия в стена Театра.jpg',
                    subtext: '26.11.2022',
                    h2: "Фотосессия в стенах Театра драмы",
                    p: "Организовывая фотосессию для локального бренда одежды мы смогли воплотить все пожелания заказчика и у нас получилась отличная работа. Смотрите как это было "
                },
            ]
        }
    }
}
</script>


<style lang="scss">
.items_block{
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 60px;
    .item_block{
        display: flex;
        align-items: flex-end;
        margin-bottom: 60px;
        .slider_text{
            margin-left: 60px;
            height: 291px;
            .slider_text_doun{
                margin-top: 40px;
                display: flex;
                align-items: center;
                justify-content: space-between;
            }
            .slider_text_up{
                margin-bottom:70px ;
            }
        }
    }
    

}


</style>