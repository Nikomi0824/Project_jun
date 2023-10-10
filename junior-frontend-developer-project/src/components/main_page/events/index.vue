<template>
    <div class="wite_bagrounde">
        <h2>МЕРОПРИЯТИЯ</h2>
        <swiper class="contener" :options="constructions">
            <swiper-slide class="items_slider" v-for="(item, index) in items" :key="index">
                <div>
                    <img :src="item.img" alt="">
                    <p>{{ item.h2 }}</p>
                    <p class="slider_center">{{ item.text }}</p>
                    <p>{{ item.subtext }}</p>
                </div>
            </swiper-slide>
        </swiper>

        <div class="management_swiper">
            <div>
                <button class="img-button left">
                    <img src="/Image/link (2).svg" alt="">
                </button>
            </div>

            <div class="swiper-pagination"></div>

            <div>
                <button class="img-button right">
                    <img src="/Image/link (2).svg" alt="">
                </button>
            </div>
        </div>
        
        <router-link to="" class="contener text-button under_slider">Смотреть все</router-link>
        
    </div>
</template>

<script>

import { Swiper, SwiperSlide  } from 'vue-awesome-swiper';
import 'swiper/css/swiper.css';


export default {
    name: 'SliderBlock',
    data(){
        return{
            items:[
                  {
                    img:"/Image/Nirvana.jpg",
                    h2:"Собираемся и слушаем альбом Nirvana. Nirvana",
                    text:"Это третий альбом группы, выпущенный после смерти Курта Кобейна и первый, содержащий студийный материал.",
                    subtext:"16.12.2021 | начало 18.00"
                },
                  {
                    img: "/Image/Nirvana.jpg",
                    h2: "Собираемся и слушаем альбом Nirvana. Nirvana",
                    text: "Это третий альбом группы, выпущенный после смерти Курта Кобейна и первый, содержащий студийный материал.",
                    subtext: "16.12.2021 | начало 18.00"
                },
                  {
                    img: "/Image/Nirvana.jpg",
                    h2: "Собираемся и слушаем альбом Nirvana. Nirvana",
                    text: "Это третий альбом группы, выпущенный после смерти Курта Кобейна и первый, содержащий студийный материал.",
                    subtext: "16.12.2021 | начало 18.00"
                },
                  {
                    img: "/Image/Nirvana.jpg",
                    h2: "Собираемся и слушаем альбом Nirvana. Nirvana",
                    text: "Это третий альбом группы, выпущенный после смерти Курта Кобейна и первый, содержащий студийный материал.",
                    subtext: "16.12.2021 | начало 18.00"
                },
                  {
                    img: "/Image/Nirvana.jpg",
                    h2: "Собираемся и слушаем альбом Nirvana. Nirvana",
                    text: "Это третий альбом группы, выпущенный после смерти Курта Кобейна и первый, содержащий студийный материал.",
                    subtext: "16.12.2021 | начало 18.00"
                },
            ]
                
            
        }
    },
    components: {
        Swiper,
        SwiperSlide,
        
    },
    computed: {
       
        constructions() {
            return {
                slidesPerView: 3,
                spaceBetween: 60,
                slidesPerGroup: 1,
                loop: true,
                loopFillGroupWithBlank: true,
                pagination: {
                    el: '.swiper-pagination',
                    clickable: true,
                    
                },
                navigation: {
                    nextEl: '.right',
                    prevEl: '.left',
                },
                  breakpoints: {
                    600: {
                        slidesPerView: 3,
                        spaceBetween: 60
                    },
                    60:{
                        slidesPerView: 1,
                        spaceBetween: 60
                    }

                }
            };
        },
    },
};
</script>

<style lang="scss" scoped>
.wite_bagrounde {
    clip-path: polygon(0.00% 0.02%, 35.31% 2.92%, 100.00% 0.00%, 100.00% 100%, 69.44% 97.23%, 0.00% 100%);
    background-color: white;
    height: 1236px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    z-index: -111;
    .management_swiper{
        display: flex;
        width: 35%;
        justify-content: space-around;
        align-items: center;
        .left{
            transform: rotate(180deg);
        }
        .swiper-pagination {
            display: flex;
            justify-content:space-around;    
            width: 99px;
        }
    }   
    .under_slider{
        text-align: end;
        border: none;
    }
}
.items_slider{
    width: 30%;
    height: 612px;
    text-align: start;
    img{
       width: 100%;
        height: 434px;
        object-fit: cover;
        margin-bottom: 20px;
    }
    p{
        width: 100%;
    }
    .slider_center{
        margin: 8px 0;
    }
}
.swiper-pagination ::v-deep{
    .swiper-pagination-bullet{
        width: 15px;
        height: 2px;
        border-radius: 10px;
        border: white solid 1px;
        background-color: #BFBFBF;
    }
    
    .swiper-pagination-bullet-active{
        background-color: black;
    }

}
 
</style>