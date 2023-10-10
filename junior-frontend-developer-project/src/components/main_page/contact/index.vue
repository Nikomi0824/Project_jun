<template>
    <div>
        <h2>контакты</h2>
        <div class="contener contact">
            <div class="contact_items">
                <div class="contact_item" v-for="(item, index) in items" :key="index">
                    <img :src="item.img">
                    <div class="contact_items_text">
                        <p>{{ item.p1 }}</p>
                        <p>{{ item.p2 }}</p>
                        <p>{{ item.p3 }}</p>
                    </div>
                </div>
            </div>
            <img  src="/Image/Frame 1994 1.svg" alt="">
        </div>
    </div>
</template>


<script>

export default{
    name:"ContactBlock",
    
    data(){
        return{
            items:[
                {
                    img:'/Image/location.svg',
                    p1: 'Томск, Белая 8',
                    p2: '2 этаж',
                    p3: 'оф. 207-208'
                    
                },
                {
                    img: '/Image/home.svg',
                    p1: 'Отдел аренды ',
                    p2: '+7 499 350 0730',
                    p3: 'hi@tagree.ru'
                },
                {
                    img: '/Image/star (1).svg',
                    p1: 'Отдел мероприятий ',
                    p2:'+7 499 350 0730',
                    p3:'hi@tagree.ru'
                },
            ]
        }
    }
}

</script>


<style lang="scss">
.contact{
    display:flex;
    justify-content: space-between;
    .contact_items{
        display:flex;
        flex-direction: column;
        justify-content: space-between;
        width: 50%;
        .contact_item{
            display:flex;
            .contact_items_text{
                display: flex;
                justify-content: space-around;
                flex-direction: column;
                margin-left: 54px;
                width: 50%;
            }
        }
        
    }
}
</style>