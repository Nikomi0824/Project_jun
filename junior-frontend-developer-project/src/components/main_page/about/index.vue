<template>
    <div class="content contener">
      <h2>О нас</h2>
      <div class="start"><p>Проект «Millennials»</p></div>
      <div class="end">
        <p>
          Вдохновлен молодыми идейными людьми, увлеченными творчеством, эмоциями и
          желанием сделать мир лучше, проявить себя. У них есть талант и стремление,
          у нас возможность помочь им воплотить их мечту в реальность.
        </p>
      </div>
      <img class="img_one" src="/Image/pic.svg" alt="" />
      <img class="img_two" src="/Image/pic (1).svg" alt="" />
      <div class="start">
        <p>Мы предоставляем площади для вашего мероприятия</p>
      </div>
      <div class="end">
        <p>
          И оказываем помощь с организацией, если вам это нужно.<br />Наша цель:
          вовлечь в культурную жизнь города как можно больше людей, помочь молодым
          ребятам сделать первые шаги к своей мечте и рассказать всем о том, что их
          волнует.
        </p>
      </div>
      <ItemBlock class="ItemBlock"></ItemBlock>
    </div>
</template>


<script>
import ItemBlock from "./item.vue"
export default{
    name:"AboutBlock",
    components:{
        ItemBlock
    }
}
</script>

<style lang="scss">
.content{
    position: relative;
    p{
        width: 50%;
    }
    .start{
        display: flex;
        align-items: flex-start;
        justify-content: flex-start;

    }
    .end{
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        margin-top: 50px;
    }
    .ItemBlock{
        margin-top: 110px;
    }
    .img_one{
        margin: 100px 0;
        width: 65%;
        height: 577px;
    }
    .img_two{
        width: 30%;
        height: 535.971px;
        position: absolute;
        top: 600px;
        right: 0;
        
    }
}
</style>

