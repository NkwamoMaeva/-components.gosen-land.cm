<template>
  <div id="header-carousel">
    <div class="header-carousel-navigation">
      <v-btn
        fab
        class="header-carousel-navigation-button active header-carousel-navigation-left"
        height="60"
        width="60"
        @click="prev"
      >
        <v-icon
          size="66"
          color="#fff"
        >
          keyboard_arrow_left
        </v-icon>
      </v-btn>
      <v-btn
        fab
        class="header-carousel-navigation-button header-carousel-navigation-right"
        height="60"
        width="60"
        @click="next"
      >
        <v-icon
          size="66"
          color="#fff"
        >
          keyboard_arrow_right
        </v-icon>
      </v-btn>
    </div>
    <div class="header-carousel-slides">
      <header-carousel-item
        v-for="(v, k) in slides"
        :key="k"
        class="header-carousel-slides-item"
        :index="k"
        :slide="v"
      />
    </div>
  </div>
</template>

<script>
import HeaderCarouselItem from "@/components/home-header/right/header-carousel/HeaderCarouselItem";
export default {
  name: "HeaderCarousel",
  components: {HeaderCarouselItem},
  props: {
    slides: {
      type: Array,
      required: true
    }
  },
  data: () => ({
    index: 0
  }),
  methods: {
    next () {
      this.index++
      if (this.index >= this.slides.length) {
        this.index = 0
      }
    },
    prev () {
      this.index--
      if (this.index < 0) {
        this.index = this.slides.length - 1
      }
    }
  }
}
</script>

<style lang="scss" scoped>
  #header-carousel{
    width: 100%;
    position: relative;
    .header-carousel-navigation{
      position: absolute;
      z-index: 1;
      top: 50%;
      transform: translateX(-50%);
      .header-carousel-navigation-button{
        background: #a3b9b8;
        &:first-child{
          margin-right: 60px;
        }
      }
      .header-carousel-navigation-button.active{
        background: transparent linear-gradient(180deg, #00BFA6 0%, #288E45 100%) 0 0 no-repeat padding-box;
      }
    }
    .header-carousel-slides{
      display: flex;
      flex-wrap: nowrap;
      width: auto;
    }
  }
</style>
