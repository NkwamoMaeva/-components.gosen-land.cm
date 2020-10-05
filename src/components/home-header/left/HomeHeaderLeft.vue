<template>
  <div id="home-header-left">
    <h1 class="my-simple-title">
      Acheter un terrain, ne paut se faire n'importe où
    </h1>
    <p class="my-description">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolore facere laudantium molestias mollitia necessitatibus neque nesciunt quia, rem velit voluptates. Ab amet dolorum iste maxime necessitatibus quisquam sed voluptatem, voluptatum.
    </p>
    <home-header-form />
  </div>
</template>

<script>
import HomeHeaderForm from "@/components/home-header/left/HomeHeaderForm";
export default {
name: "HomeHeaderLeft",
  components: {HomeHeaderForm}
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@100;200;300;400;500;700&display=swap');

  #home-header-left{
    margin-left: 80px;
    .my-simple-title{
      font: normal normal 500 60px/70px Raleway;
      font-weight: 500;
      color: #288E45;
      margin-bottom: 17px;
    }
    .my-description{
      font: normal normal normal 25px/30px Raleway;
      color: #545454;
      margin-bottom: 50px;
    }
  }
</style>
