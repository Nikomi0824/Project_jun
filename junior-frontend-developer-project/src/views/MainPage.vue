<template>
    <div>
        <MainBlock></MainBlock>
        <AboutBlock></AboutBlock>
        <SliderBlock></SliderBlock>
        <BlogBlock></BlogBlock>
        <ContactBLock></ContactBLock>
        <TextBlock></TextBlock>
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