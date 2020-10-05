<template>
  <div id="header-carousel-item">
    <div
      class="header-carousel-item"
      :style="{background: `url('${slide.img}') center no-repeat`}"
    />
  </div>
</template>

<script>
export default {
  name: "HeaderCarouselItem",
  props: {
    slide: {
      type: Object,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
#header-carousel-item{
  //filter: drop-shadow(-1px 6px 3px rgba(0,0,0,.5));
  width: 100%;
  flex-shrink: 0;
  .header-carousel-item{
    background-size: cover!important;
    clip-path: polygon(0% 0%, 100% 0%, 100% 100%, 0% 93%);
    width: 100%;
    height: 734px;
    border-radius: 15px 0 0 0;
  }
}
</style>
