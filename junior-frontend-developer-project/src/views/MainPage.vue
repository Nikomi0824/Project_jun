<template>
    <div>
        <MainBlock class="MainBlock"></MainBlock>
        <AboutBlock class="AboutBlock"></AboutBlock>
        <SliderBlock class="SliderBlock"></SliderBlock>
        <BlogBlock class="BlogBlock"></BlogBlock>
        <ContactBLock class="ContactBLock"></ContactBLock>
        <TextBlock class="TextBlock"></TextBlock>
    </div>
</template>


<script>
import MainBlock from "@/components/main_page/mainBlock/index.vue"
import AboutBlock from "@/components/main_page/about/index.vue"
import SliderBlock from "@/components/main_page/events/index.vue"
import BlogBlock from "@/components/main_page/blog/index.vue"
import ContactBLock from "@/components/main_page/contact/index.vue"
import TextBlock from "@/components/main_page/text/index.vue"
export default{
    name:"MainPage",
    components:{
        MainBlock,
        AboutBlock,
        SliderBlock,
        BlogBlock,
        ContactBLock,
        TextBlock
        
    }
}

</script>


<style>
.MainBlock{
    margin-top: 200px;
}
.AboutBlock{
    margin-top: 208px;
}
.SliderBlock{
    margin-top: 90px;
}
.BlogBlock{
    margin-top: 70px;
}
.ContactBLock{
    margin-top: 86px;
}
.TextBlock{
    margin: 150px 0 254px;
}
</style>