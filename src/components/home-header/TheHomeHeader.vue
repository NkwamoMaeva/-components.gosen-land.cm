<template>
  <div id="the-home-header">
    <home-header-left class="the-home-header-left" />
    <home-header-right class="the-home-header-right" />
  </div>
</template>

<script>
import HomeHeaderLeft from "@/components/home-header/left/HomeHeaderLeft";
import HomeHeaderRight from "@/components/home-header/right/HomeHeaderRight";
export default {
name: "TheHomeHeader",
  components: {HomeHeaderRight, HomeHeaderLeft}
}
</script>

<style lang="scss" scoped>
#the-home-header{
  display: flex;
  align-items: center;
  .the-home-header-left{
    width: calc(60% - 50px);
    margin-right: 50px;
  }
  .the-home-header-right{
    width: calc(40% - 50px);
    margin-left: 50px;
  }
}
</style>
