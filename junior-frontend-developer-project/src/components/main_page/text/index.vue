<template>
    <div class="text_block">
        <img class="text_block1" src="/Image/Просто делайте, что нравится,.svg" alt="">
        <div class="text_block2">
            <img  src="/Image/а мы вам поможем.svg" alt="">
        </div>
    </div>
</template>

<script>
export default{
    name:"TextBlock"
}
</script>

<style lang="scss">
.text_block{
    width: 100%;

    .text_block1{
        width: 100%;
    }
    .text_block2{
        img{
            position: absolute;
            width: 63%;
            right: 0;
        }
        
    }
}

</style>