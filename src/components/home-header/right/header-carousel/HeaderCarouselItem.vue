<template>
  <div
    v-show="visible"
    id="header-carousel-item"
  >
    <div
      class="header-carousel-item"
      :style="{background: `url('${slide.img}') center no-repeat`}"
    />
    <div class="header-carousel-item-content">
      <div class="header-carousel-item-description">
        <div class="header-carousel-item-description-header">
          <div class="header-carousel-item-description-header-location">
            <v-icon>home</v-icon>
            <span>Douala (Ndogbong)</span>
          </div>
          <div class="header-carousel-item-description-header-dim">
            <v-icon>home</v-icon>
            <span>120 km²</span>
          </div>
          <p class="header-carousel-item-description-header-descr">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam delectus est excepturi iure sapiente voluptates! Est, omnis, quos. Amet aperiam distinctio eaque facilis illo itaque laudantium obcaecati repellat sapiente vitae?
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderCarouselItem",
  props: {
    slide: {
      type: Object,
      required: true
    },
    index: {
      type: Number,
      required: true
    }
  },
  computed: {
    /**
     * Retourne la visibilité de la slide
     */
    visible () {
      return this.index === this.$parent.index
    }
  }
}
</script>

<style lang="scss" scoped>
#header-carousel-item{
  //filter: drop-shadow(-1px 6px 3px rgba(0,0,0,.5));
  width: 100%;
  flex-shrink: 0;
  position: relative;
  .header-carousel-item{
    background-size: cover!important;
    clip-path: polygon(0% 0%, 100% 0%, 100% 100%, 0% 93%);
    width: 100%;
    height: 734px;
    border-radius: 15px 0 0 0;
  }
  .header-carousel-item-content{
    position: absolute;
    z-index: 1;
    top: 0;
    filter: drop-shadow(0px 4px 10px #00000029);
    .header-carousel-item-description{
      clip-path: polygon(0% 0%, 100% 0%, 100% 87%, 0% 99%);
      background: #FFFFFF 0% 0% no-repeat padding-box;
      width: 340px;
      height: 230px;
      border-radius: 20px;
      padding: 25px;
    }
  }
}
</style>
