<template>
  <div id="app">
    <HeaderBlock></HeaderBlock>
    <router-view/>
    <FooterBlock class="FooterBlock"></FooterBlock>
    <img class="bagarunde" src="/Image/bagraund.svg" alt="">
  </div>
</template>

<script>
import HeaderBlock from "@/components/header/index.vue"
import FooterBlock from "@/components/footer/index.vue"
export default{
  components:{
    HeaderBlock,
    FooterBlock
  }
}
</script>

<style lang="scss">
@import url("./assets/Style/global.scss");
#app {
  background: "@/assets/Image/bagraund.svg";
  
}
.FooterBlock{
  margin-top: 100px;
  
}
.bagarunde{
  position: absolute;
  top:0;
  z-index: -111111;
  width: 100%;
}
</style>
